---
title: recurso educationSynchronizationOAuth2ClientCredentialsConnectionSettings
description: Quando a concessão de credenciais de cliente do OAuth2 for usada para se conectar ao provedor de dados, esse tipo de configuração de conexão deverá ser usado para configurar o perfil.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d38853e40d8f88bf4aa8323395848185793cc42c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500090"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="5aa12-103">recurso educationSynchronizationOAuth2ClientCredentialsConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="5aa12-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

<span data-ttu-id="5aa12-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5aa12-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5aa12-105">Quando a [concessão de credenciais de cliente do OAuth2](https://tools.ietf.org/html/rfc6749#section-4.4) for usada para se conectar ao provedor de dados, esse tipo de configuração de conexão deverá ser usado para configurar o perfil.</span><span class="sxs-lookup"><span data-stu-id="5aa12-105">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="5aa12-106">Derivado de [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span><span class="sxs-lookup"><span data-stu-id="5aa12-106">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5aa12-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5aa12-107">Properties</span></span>

| <span data-ttu-id="5aa12-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5aa12-108">Property</span></span> | <span data-ttu-id="5aa12-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5aa12-109">Type</span></span> | <span data-ttu-id="5aa12-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5aa12-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="5aa12-111">**tokenUrl**</span><span class="sxs-lookup"><span data-stu-id="5aa12-111">**tokenUrl**</span></span> | <span data-ttu-id="5aa12-112">String</span><span class="sxs-lookup"><span data-stu-id="5aa12-112">String</span></span> | <span data-ttu-id="5aa12-113">A URL para obter tokens de acesso para o provedor de dados.</span><span class="sxs-lookup"><span data-stu-id="5aa12-113">The URL to get access tokens for the data provider.</span></span> |
| <span data-ttu-id="5aa12-114">**scope**</span><span class="sxs-lookup"><span data-stu-id="5aa12-114">**scope**</span></span> | <span data-ttu-id="5aa12-115">String</span><span class="sxs-lookup"><span data-stu-id="5aa12-115">String</span></span> | <span data-ttu-id="5aa12-116">[O escopo da solicitação de acesso](https://tools.ietf.org/html/rfc6749#section-3.3).</span><span class="sxs-lookup"><span data-stu-id="5aa12-116">[The scope of the access request](https://tools.ietf.org/html/rfc6749#section-3.3).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5aa12-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5aa12-117">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings",
    "clientId": "String",
    "clientSecret": "String",
    "tokenUrl": "String",
    "scope": "String"
}
```
