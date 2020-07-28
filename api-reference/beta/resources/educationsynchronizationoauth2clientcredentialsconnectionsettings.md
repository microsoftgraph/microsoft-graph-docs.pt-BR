---
title: recurso educationSynchronizationOAuth2ClientCredentialsConnectionSettings
description: Quando a concessão de credenciais de cliente do OAuth2 for usada para se conectar ao provedor de dados, esse tipo de configuração de conexão deverá ser usado para configurar o perfil.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 00e1e531ff33f28a2e63f76925cd0b4e7759696b
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434904"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="d7393-103">recurso educationSynchronizationOAuth2ClientCredentialsConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="d7393-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

<span data-ttu-id="d7393-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7393-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7393-105">Quando a [concessão de credenciais de cliente do OAuth2](https://tools.ietf.org/html/rfc6749#section-4.4) for usada para se conectar ao provedor de dados, esse tipo de configuração de conexão deverá ser usado para configurar o perfil.</span><span class="sxs-lookup"><span data-stu-id="d7393-105">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="d7393-106">Derivado de [educationSynchronizationConnectionSettings].</span><span class="sxs-lookup"><span data-stu-id="d7393-106">Derived from [educationSynchronizationConnectionSettings].</span></span>

## <a name="properties"></a><span data-ttu-id="d7393-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d7393-107">Properties</span></span>

| <span data-ttu-id="d7393-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d7393-108">Property</span></span>     | <span data-ttu-id="d7393-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7393-109">Type</span></span>   | <span data-ttu-id="d7393-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7393-110">Description</span></span>                                                                                                                |
| :----------- | :----- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="d7393-111">clientId</span><span class="sxs-lookup"><span data-stu-id="d7393-111">clientId</span></span>     | <span data-ttu-id="d7393-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7393-112">String</span></span> | <span data-ttu-id="d7393-113">ID do cliente usada para se conectar ao provedor.</span><span class="sxs-lookup"><span data-stu-id="d7393-113">Client ID used to connect to the provider.</span></span> <span data-ttu-id="d7393-114">Herdado de [educationSynchronizationConnectionSettings].</span><span class="sxs-lookup"><span data-stu-id="d7393-114">Inherited from [educationSynchronizationConnectionSettings].</span></span>                    |
| <span data-ttu-id="d7393-115">clientSecret</span><span class="sxs-lookup"><span data-stu-id="d7393-115">clientSecret</span></span> | <span data-ttu-id="d7393-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7393-116">String</span></span> | <span data-ttu-id="d7393-117">Segredo do cliente para autenticar a conexão com o provedor.</span><span class="sxs-lookup"><span data-stu-id="d7393-117">Client secret to authenticate the connection to the provider.</span></span> <span data-ttu-id="d7393-118">Herdado de [educationSynchronizationConnectionSettings].</span><span class="sxs-lookup"><span data-stu-id="d7393-118">Inherited from [educationSynchronizationConnectionSettings].</span></span> |
| <span data-ttu-id="d7393-119">tokenUrl</span><span class="sxs-lookup"><span data-stu-id="d7393-119">tokenUrl</span></span>     | <span data-ttu-id="d7393-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7393-120">String</span></span> | <span data-ttu-id="d7393-121">A URL para obter tokens de acesso para o provedor de dados.</span><span class="sxs-lookup"><span data-stu-id="d7393-121">The URL to get access tokens for the data provider.</span></span>                                                                        |
| <span data-ttu-id="d7393-122">escopo</span><span class="sxs-lookup"><span data-stu-id="d7393-122">scope</span></span>        | <span data-ttu-id="d7393-123">String</span><span class="sxs-lookup"><span data-stu-id="d7393-123">String</span></span> | <span data-ttu-id="d7393-124">O escopo da solicitação de acesso (consulte [RFC6749](https://tools.ietf.org/html/rfc6749#section-3.3)).</span><span class="sxs-lookup"><span data-stu-id="d7393-124">The scope of the access request (see [RFC6749](https://tools.ietf.org/html/rfc6749#section-3.3)).</span></span>                          |

[educationsynchronizationconnectionsettings]: educationsynchronizationconnectionsettings.md

## <a name="json-representation"></a><span data-ttu-id="d7393-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d7393-126">JSON representation</span></span>

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
