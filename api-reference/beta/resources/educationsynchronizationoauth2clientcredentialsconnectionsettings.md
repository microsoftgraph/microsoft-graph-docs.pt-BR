---
title: recurso educationSynchronizationOAuth2ClientCredentialsConnectionSettings
description: Quando a concessão de credenciais de cliente do OAuth2 for usada para se conectar ao provedor de dados, esse tipo de configuração de conexão deverá ser usado para configurar o perfil.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 5b0229ae431c02f85d393ff80b0bba32e32683c9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334021"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="0f44b-103">recurso educationSynchronizationOAuth2ClientCredentialsConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="0f44b-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f44b-104">Quando a [concessão de credenciais de cliente do OAuth2](https://tools.ietf.org/html/rfc6749#section-4.4) for usada para se conectar ao provedor de dados, esse tipo de configuração de conexão deverá ser usado para configurar o perfil.</span><span class="sxs-lookup"><span data-stu-id="0f44b-104">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="0f44b-105">Derivado de [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span><span class="sxs-lookup"><span data-stu-id="0f44b-105">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0f44b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0f44b-106">Properties</span></span>

| <span data-ttu-id="0f44b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f44b-107">Property</span></span> | <span data-ttu-id="0f44b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f44b-108">Type</span></span> | <span data-ttu-id="0f44b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f44b-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="0f44b-110">**tokenUrl**</span><span class="sxs-lookup"><span data-stu-id="0f44b-110">**tokenUrl**</span></span> | <span data-ttu-id="0f44b-111">String</span><span class="sxs-lookup"><span data-stu-id="0f44b-111">String</span></span> | <span data-ttu-id="0f44b-112">A URL para obter tokens de acesso para o provedor de dados.</span><span class="sxs-lookup"><span data-stu-id="0f44b-112">The URL to get access tokens for the data provider.</span></span> |
| <span data-ttu-id="0f44b-113">**scope**</span><span class="sxs-lookup"><span data-stu-id="0f44b-113">**scope**</span></span> | <span data-ttu-id="0f44b-114">String</span><span class="sxs-lookup"><span data-stu-id="0f44b-114">String</span></span> | <span data-ttu-id="0f44b-115">[O escopo da solicitação de acesso](https://tools.ietf.org/html/rfc6749#section-3.3).</span><span class="sxs-lookup"><span data-stu-id="0f44b-115">[The scope of the access request](https://tools.ietf.org/html/rfc6749#section-3.3).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0f44b-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0f44b-116">JSON representation</span></span>
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
