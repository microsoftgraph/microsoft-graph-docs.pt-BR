---
title: tipo de recurso educationSynchronizationConnectionSettings
description: 'Representa as configurações de conexão do provedor. Isso permite que o sistema saiba como se conectar às APIs do provedor. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9d972aec91218dfc9606da4c8aa88e27b63167d9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500566"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a>tipo de recurso educationSynchronizationConnectionSettings

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações de conexão do provedor. Isso permite que o sistema saiba como se conectar às APIs do provedor. 

> **Observação:** Esse tipo complexo é abstrato. Consulte os tipos específicos de configurações de conexão listadas.

## <a name="derived-types"></a>Tipos derivados
| Tipo | Descrição | 
|:-|:-|
| [**educationSynchronizationOAuth1ConnectionSettings**](educationsynchronizationoauth1connectionsettings.md) | Use este tipo para fornecer configurações de conexão do OAuth1. |
| [**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | Use este tipo para fornecer as configurações de conexão de credenciais de cliente do OAuth2. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **clientId** | String |  ID do cliente usada para se conectar ao provedor. |
| **clientSecret** | String |  Segredo do cliente para autenticar a conexão com o provedor. |
