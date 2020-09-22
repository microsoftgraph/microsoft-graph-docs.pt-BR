---
title: recurso educationPowerSchoolDataProvider
description: Usado para configurar o perfil de sincronização de dados da escola quando PowerSchool é usado como a fonte de entrada.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 664b7c9c3ad255e502583fca6be332043e712a46
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979613"
---
# <a name="educationpowerschooldataprovider-resource"></a>recurso educationPowerSchoolDataProvider

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado para configurar o perfil de sincronização de dados da escola quando [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) é usado como a fonte de entrada.

Derivado de [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).

## <a name="properties"></a>Propriedades

| Propriedade                       | Tipo                                     | Descrição                                                                            |
| :----------------------------- | :--------------------------------------- | :------------------------------------------------------------------------------------- |
| allowTeachersInMultipleSchools | Boolean                                  | Indica se a fonte tem vários identificadores para um único aluno ou professor. |
| clientId                       | Cadeia de caracteres                                   | A ID do cliente usada para se conectar ao PowerSchool.                                          |
| clientSecret                   | Cadeia de caracteres                                   | O segredo do cliente para autenticar a conexão com a instância do PowerSchool.          |
| connectionUrl                  | String                                   | A URL de conexão para a instância do PowerSchool.                                        |
| schoolsIds                     | Coleção de cadeias de caracteres                        | A lista de escolas a ser sincronizada.                                                           |
| schoolYear                     | String                                   | O ano escolar a ser sincronizado.                                                               |
| personalizações                 | [educationSynchronizationCustomizations] | Personalização opcional a ser aplicada ao perfil de sincronização.                   |

[educationsynchronizationconnectionsettings]: educationsynchronizationconnectionsettings.md
[educationsynchronizationcustomizations]: educationsynchronizationcustomizations.md

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
  "customizations": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
  }
}
```


