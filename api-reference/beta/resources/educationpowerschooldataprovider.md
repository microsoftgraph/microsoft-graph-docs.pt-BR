---
title: recurso educationPowerSchoolDataProvider
description: Usado para configurar o perfil de sincronização de dados da escola quando PowerSchool é usado como a fonte de entrada.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4fda7cc98c8041aad45a0ef8453affc9af34edc5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501224"
---
# <a name="educationpowerschooldataprovider-resource"></a>recurso educationPowerSchoolDataProvider

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado para configurar o perfil de sincronização de dados da escola quando [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) é usado como a fonte de entrada.

Derivado de [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **connectionUrl** | String | A URL de conexão para a instância do PowerSchool. |
| **clientId** | String |  A ID do cliente usada para se conectar ao PowerSchool. |
| **clientSecret** | String |  O segredo do cliente para autenticar a conexão com a instância do PowerSchool. |
| **schoolsIds** | String collection |  A lista de escolas a ser sincronizada. |
| **schoolYear** | String |  O ano escolar a ser sincronizado. |
| **allowTeachersInMultipleSchools** | Boolean |  Indica se a fonte tem vários identificadores para um único aluno ou professor. |
| **personalizações** | [educationSynchronizationCustomizations](educationsynchronizationcustomizations.md) | Personalização opcional a ser aplicada ao perfil de sincronização.|

## <a name="json-representation"></a>Representação JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPowerSchoolDataProvider"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationPowerSchoolDataProvider",
  "connectionUrl": "String",
  "clientId": "String",
  "clientSecret": "String",
  "schoolsIds": ["String"],
  "schoolYear": "String",
  "allowTeachersInMultipleSchools": "Boolean",
  "customizations": {"@odata.type": "microsoft.graph.educationSynchronizationCustomizations"}
}
```
