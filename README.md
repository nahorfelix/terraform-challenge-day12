# Day 12 — Zero-Downtime Deployments

This folder is a **placeholder** in the local workspace so Day 12 stays easy to find next to Days 9–11 and 14–16.

## Curriculum (Day 12)

- `create_before_destroy` on launch template / ASG  
- ASG **name uniqueness** (`name_prefix` or `random_id`)  
- Optional: blue/green listener rules; `curl` loop during `apply`

## Where the patterns live in this workspace

| Pattern | Location |
|--------|----------|
| `create_before_destroy`, `name_prefix` on ASG | `terraform-challenge-day16/modules/webserver-cluster/asg.tf` (also in `terraform-challenge-day11` / `terraform-challenge-day9` webserver modules) |
| ELB health checks | Same webserver cluster modules |

## Free tier

Keep ASG **min/max** small; **destroy** when finished.

---

If you need a separate Git repo for submissions, copy the module from Day 16 or Day 11 and trim to only zero-downtime experiments.
