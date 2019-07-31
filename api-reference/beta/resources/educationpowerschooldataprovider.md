---
title: recurso educationPowerSchoolDataProvider
description: Usado para configurar o perfil de sincronização de dados da escola quando PowerSchool é usado como a fonte de entrada.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 6a036435cb7cc1a4ef70960b09feb600fe7f39f8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972590"
---
# <a name="educationpowerschooldataprovider-resource"></a>recurso educationPowerSchoolDataProvider

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado para configurar o perfil de sincronização de dados da escola quando [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) é usado como a fonte de entrada.

Derivado de [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **connectionUrl** | String | A URL de conexão para a instância do PowerSchool. |
| **clientId** | String |  A ID do cliente usada para se conectar ao PowerSchool. |
| **clientSecret** | String |  O segredo do cliente para autenticar a conexão com a instância do PowerSchool. |
| **schoolsIds** | Coleção de cadeias de caracteres |  A lista de escolas a ser sincronizada. |
| **schoolYear** | String |  O ano escolar a ser sincronizado. |
| **allowTeachersInMultipleSchools** | Booliano |  Indica se a fonte tem vários identificadores para um único aluno ou professor. |
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
