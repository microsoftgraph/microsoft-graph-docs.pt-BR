---
title: recurso de educationPowerSchoolDataProvider
description: Usado para configurar o perfil de sincronização de dados da escola quando PowerSchool é usado como a fonte de entrada.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 4028170c2780cee426ec961a44b51e0362b0187f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406917"
---
# <a name="educationpowerschooldataprovider-resource"></a>recurso de educationPowerSchoolDataProvider

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Usado para configurar o perfil de sincronização de dados da escola quando [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) é usado como a fonte de entrada.

Derivado do [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **URL de conexão** | String | A URL da conexão para a instância de PowerSchool. |
| **clientId** | String |  A identificação do cliente usada para conectar ao PowerSchool. |
| **clientSecret** | String |  O segredo do cliente para autenticar a conexão à instância PowerSchool. |
| **schoolsIds** | String collection |  A lista de escolas para sincronizar. |
| **schoolYear** | String |  O ano escola para sincronizar. |
| **allowTeachersInMultipleSchools** | Boolean |  Indica se a fonte tem vários identificadores para um único aluno ou professor. |
| **personalizações** | [educationSynchronizationCustomizations](educationsynchronizationcustomizations.md) | Personalização opcional a ser aplicado ao perfil de sincronização.|

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
    "schoolsids": ["String"],
    "schoolYear": "String",
    "allowTeachersInMultipleSchools": "Boolean",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
