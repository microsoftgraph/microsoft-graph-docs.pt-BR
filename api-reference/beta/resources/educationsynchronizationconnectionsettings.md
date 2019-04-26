---
title: tipo de recurso educationSynchronizationConnectionSettings
description: 'Representa as configurações de conexão do provedor. Isso permite que o sistema saiba como se conectar às APIs do provedor. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 387c002240d54d1ec12e58564e91831d6f0e8a50
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334099"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a>tipo de recurso educationSynchronizationConnectionSettings

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
