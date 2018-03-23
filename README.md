```sh

mvn dependency:copy -Dartifact=io.swagger:swagger-codegen-cli:2.2.2 -DoutputDirectory=. -Dmdep.stripVersion=true

java -jar swagger-codegen-cli.jar generate   -i http://petstore.swagger.io/v2/swagger.json   --api-package com.baeldung.petstore.client.api   --model-package com.baeldung.petstore.client.model   --invoker-package com.baeldung.petstore.client.invoker   --group-id com.baeldung   --artifact-id bc-api   --artifact-version 0.0.1-SNAPSHOT   -l spring   -o bc-api

```
