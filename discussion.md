20/12/23

None of this is final.

postponed most of the incremental updates discussion to focus on the datamodel
    incremental updates should not exclude transferring complete ecs as file -> squash incremental updates
started out discussing how to define a wall with two windows making a void in the wall

data model specification process in json, final serialization tbd, some favor for binary
view strange matter as transfer format, and as source of truth, not primarily as database
which parts of ECS do we care about, so far S excluded, maybe data driven design as well

relation to component or entity? favor for entity
use tags/status in component header to specify component types further?
components have hash as unique identifier
types are expressed as relationship to type entity, and should not be called types
    flatting the ecs needs to happen at some point, export/import/query, by including types in the ecs we are retaining the type semantics of the authoring app more accurately, but need to find terminology that works better for ECS
deciding the identity of objects should play central role in data model design
ownership is on component instance level, not on component type level
    allows stakeholder to, for instance, add void relationships to wall without owning all those relationships, or the relationship component type
use namespaces to scope what is ifc and what is extension

include authoring information as metadata or within ecs? git approach -> metadata, ifc2/4 approach -> within ecs

