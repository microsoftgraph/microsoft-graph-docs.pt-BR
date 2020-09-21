---
title: tipo de recurso educationSynchronizationConnectionSettings
description: 'Representa as configurações de conexão do provedor. Isso permite que o sistema saiba como se conectar às APIs do provedor. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 449dc1c4265355d55e6d3ceb51fe86be9f84ac31
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979557"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a>tipo de recurso educationSynchronizationConnectionSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações de conexão do provedor. Isso permite que o sistema saiba como se conectar às APIs do provedor.

> [!NOTE]
> Esse tipo complexo é abstrato. Consulte os tipos específicos de configurações de conexão listadas.

## <a name="derived-types"></a>Tipos derivados

| Tipo                                                                                                                                      | Descrição                                                                   |
| :---------------------------------------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------- |
| [educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md)                                   | Use este tipo para fornecer configurações de conexão do OAuth1.                          |
| [educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | Use este tipo para fornecer as configurações de conexão de credenciais de cliente do OAuth2. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   | Descrição                                                   |
| :----------- | :----- | :------------------------------------------------------------ |
| clientId     | Cadeia de caracteres | ID do cliente usada para se conectar ao provedor.                    |
| clientSecret | Cadeia de caracteres | Segredo do cliente para autenticar a conexão com o provedor. |


