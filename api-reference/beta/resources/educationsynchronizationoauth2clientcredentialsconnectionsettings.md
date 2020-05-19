---
title: recurso educationSynchronizationOAuth2ClientCredentialsConnectionSettings
description: Quando a concessão de credenciais de cliente do OAuth2 for usada para se conectar ao provedor de dados, esse tipo de configuração de conexão deverá ser usado para configurar o perfil.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: dfe0a2fda8d49bd003a6ea2c23eb6a31ce619234
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289436"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="e3bee-103">recurso educationSynchronizationOAuth2ClientCredentialsConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="e3bee-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

<span data-ttu-id="e3bee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3bee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3bee-105">Quando a [concessão de credenciais de cliente do OAuth2](https://tools.ietf.org/html/rfc6749#section-4.4) for usada para se conectar ao provedor de dados, esse tipo de configuração de conexão deverá ser usado para configurar o perfil.</span><span class="sxs-lookup"><span data-stu-id="e3bee-105">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="e3bee-106">Derivado de [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span><span class="sxs-lookup"><span data-stu-id="e3bee-106">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e3bee-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e3bee-107">Properties</span></span>

| <span data-ttu-id="e3bee-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3bee-108">Property</span></span> | <span data-ttu-id="e3bee-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3bee-109">Type</span></span> | <span data-ttu-id="e3bee-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3bee-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="e3bee-111">**tokenUrl**</span><span class="sxs-lookup"><span data-stu-id="e3bee-111">**tokenUrl**</span></span> | <span data-ttu-id="e3bee-112">String</span><span class="sxs-lookup"><span data-stu-id="e3bee-112">String</span></span> | <span data-ttu-id="e3bee-113">A URL para obter tokens de acesso para o provedor de dados.</span><span class="sxs-lookup"><span data-stu-id="e3bee-113">The URL to get access tokens for the data provider.</span></span> |
| <span data-ttu-id="e3bee-114">**scope**</span><span class="sxs-lookup"><span data-stu-id="e3bee-114">**scope**</span></span> | <span data-ttu-id="e3bee-115">String</span><span class="sxs-lookup"><span data-stu-id="e3bee-115">String</span></span> | <span data-ttu-id="e3bee-116">[O escopo da solicitação de acesso](https://tools.ietf.org/html/rfc6749#section-3.3).</span><span class="sxs-lookup"><span data-stu-id="e3bee-116">[The scope of the access request](https://tools.ietf.org/html/rfc6749#section-3.3).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e3bee-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e3bee-117">JSON representation</span></span>
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
