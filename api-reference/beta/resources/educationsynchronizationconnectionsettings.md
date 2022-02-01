---
title: Tipo de recurso educationSynchronizationConnectionSettings
description: 'Representa as configurações de conexão do provedor. Isso permite que o sistema saiba como se conectar às APIs do provedor. '
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: eca233d7e375991f34bdd2b44351fe75f371fee1
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/01/2022
ms.locfileid: "62290585"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a>Tipo de recurso educationSynchronizationConnectionSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações de conexão do provedor. Isso permite que o sistema saiba como se conectar às APIs do provedor.

> [!NOTE]
> Esse tipo complexo é abstrato. Consulte os tipos específicos de configurações de conexão listados.

## <a name="derived-types"></a>Tipos derivados

| Tipo                                                                                                                                      | Descrição                                                                   |
| :---------------------------------------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------- |
| [educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md)                                   | Use esse tipo para fornecer configurações de conexão OAuth1.                          |
| [educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | Use esse tipo para fornecer credenciais de cliente OAuth2 Conceder configurações de conexão. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   | Descrição                                                   |
| :----------- | :----- | :------------------------------------------------------------ |
| clientId     | Cadeia de caracteres | ID do cliente usada para se conectar ao provedor.                    |
| clientSecret | Cadeia de caracteres | Segredo do cliente para autenticar a conexão com o provedor. |

## <a name="json-representation"></a>Representação JSON

A seguir está uma representação JSON desse recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationSynchronizationConnectionSettings"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationSynchronizationConnectionSettings",
  "clientId": "String",
  "clientSecret": "String",
}
```