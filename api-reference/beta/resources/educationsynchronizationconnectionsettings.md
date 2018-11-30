---
title: tipo de recurso de educationSynchronizationConnectionSettings
description: 'Representa as configurações de conexão do provedor. Isso permite que o sistema para saber como conectar ao provedor de APIs. '
ms.openlocfilehash: 27cdd377318d3294be9802b7cf28e940d0ada31c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037402"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a>tipo de recurso de educationSynchronizationConnectionSettings

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa as configurações de conexão do provedor. Isso permite que o sistema para saber como conectar ao provedor de APIs. 

> **Observação:** Este tipo complexo é abstrato. Consulte os tipos específicos de configurações de conexão listados.

## <a name="derived-types"></a>Tipos derivados
| Tipo | Descrição | 
|:-|:-|
| [**educationSynchronizationOAuth1ConnectionSettings**](educationsynchronizationoauth1connectionsettings.md) | Use este tipo para fornecer configurações de conexão OAuth1. |
| [**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | Use este tipo para fornecer configurações de conexão de concessão de credenciais do cliente OAuth2. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **clientId** | String |  ID do cliente usada para conexão com o provedor. |
| **clientSecret** | String |  Segredo do cliente para autenticar a conexão ao provedor. |