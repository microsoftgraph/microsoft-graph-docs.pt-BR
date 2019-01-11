---
title: tipo de recurso de educationSynchronizationConnectionSettings
description: 'Representa as configurações de conexão do provedor. Isso permite que o sistema para saber como conectar ao provedor de APIs. '
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 17fedb5094016bd3df3bd8262390eaa7eeb37537
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841766"
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
| **clientId** | Cadeia de caracteres |  ID do cliente usada para conexão com o provedor. |
| **clientSecret** | Cadeia de caracteres |  Segredo do cliente para autenticar a conexão ao provedor. |
