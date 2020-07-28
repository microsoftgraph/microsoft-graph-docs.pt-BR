---
title: tipo de recurso educationSynchronizationConnectionSettings
description: 'Representa as configurações de conexão do provedor. Isso permite que o sistema saiba como se conectar às APIs do provedor. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 71da1acbd9910757375acbc22dda63f412f459b2
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434876"
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
