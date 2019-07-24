---
title: tipo de recurso onPremisesPublishing
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ff5ca6afc76ab60ab82f045d0309832e34e8d708
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840765"
---
# <a name="onpremisespublishing-resource-type"></a><span data-ttu-id="d8ccc-103">tipo de recurso onPremisesPublishing</span><span class="sxs-lookup"><span data-stu-id="d8ccc-103">onPremisesPublishing resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8ccc-104">Um objeto **onPremisesPublishing** representa o conjunto de propriedades para publicar o [aplicativo](application.md)local.</span><span class="sxs-lookup"><span data-stu-id="d8ccc-104">An **onPremisesPublishing** object represents the set of properties for publishing of on-premises [application](application.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d8ccc-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d8ccc-105">Properties</span></span>

| <span data-ttu-id="d8ccc-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8ccc-106">Property</span></span>|<span data-ttu-id="d8ccc-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8ccc-107">Type</span></span>|<span data-ttu-id="d8ccc-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8ccc-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8ccc-109">customDomainCertificate</span><span class="sxs-lookup"><span data-stu-id="d8ccc-109">customDomainCertificate</span></span>|<span data-ttu-id="d8ccc-110">String</span><span class="sxs-lookup"><span data-stu-id="d8ccc-110">String</span></span>|<span data-ttu-id="d8ccc-111">Detalhes do certificado associado ao aplicativo quando um domínio personalizado está em uso.</span><span class="sxs-lookup"><span data-stu-id="d8ccc-111">Details of the certificate associated with the applicaiton when a custom domain is in use.</span></span> <span data-ttu-id="d8ccc-112">Nulo ao usar o domínio padrão.</span><span class="sxs-lookup"><span data-stu-id="d8ccc-112">Null when using the default domain.</span></span>|
|<span data-ttu-id="d8ccc-113">externalAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="d8ccc-113">externalAuthenticationType</span></span>|<span data-ttu-id="d8ccc-114">String</span><span class="sxs-lookup"><span data-stu-id="d8ccc-114">String</span></span>|<span data-ttu-id="d8ccc-115">Detalhes a configuração de pré-autenticação para o aplicativo os valores possíveis são: `passthru`, `aadPreAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="d8ccc-115">Details the pre-authentication setting for the application Possible values are: `passthru`, `aadPreAuthentication`.</span></span>|
|<span data-ttu-id="d8ccc-116">externalUrl</span><span class="sxs-lookup"><span data-stu-id="d8ccc-116">externalUrl</span></span>|<span data-ttu-id="d8ccc-117">String</span><span class="sxs-lookup"><span data-stu-id="d8ccc-117">String</span></span>|<span data-ttu-id="d8ccc-118">A URL externa publicada para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d8ccc-118">The published external url for the application.</span></span> <span data-ttu-id="d8ccc-119">Por exemplohttps://intranet-contoso.msappproxy.net/</span><span class="sxs-lookup"><span data-stu-id="d8ccc-119">For example https://intranet-contoso.msappproxy.net/</span></span>  |
|<span data-ttu-id="d8ccc-120">internalUrl</span><span class="sxs-lookup"><span data-stu-id="d8ccc-120">internalUrl</span></span>|<span data-ttu-id="d8ccc-121">String</span><span class="sxs-lookup"><span data-stu-id="d8ccc-121">String</span></span>|<span data-ttu-id="d8ccc-122">A URL interna do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d8ccc-122">The internal url of the application.</span></span> <span data-ttu-id="d8ccc-123">Por exemplohttps://intranet/</span><span class="sxs-lookup"><span data-stu-id="d8ccc-123">For example https://intranet/</span></span> |
|<span data-ttu-id="d8ccc-124">isOnPremPublishingEnabled</span><span class="sxs-lookup"><span data-stu-id="d8ccc-124">isOnPremPublishingEnabled</span></span>|<span data-ttu-id="d8ccc-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="d8ccc-125">Boolean</span></span>|<span data-ttu-id="d8ccc-126">Indica se o aplicativo está sendo publicado ou não no momento.</span><span class="sxs-lookup"><span data-stu-id="d8ccc-126">Indicates if the application is currently being published or not.</span></span>|
|<span data-ttu-id="d8ccc-127">applicationServerTimeout</span><span class="sxs-lookup"><span data-stu-id="d8ccc-127">applicationServerTimeout</span></span>|<span data-ttu-id="d8ccc-128">String</span><span class="sxs-lookup"><span data-stu-id="d8ccc-128">String</span></span>|<span data-ttu-id="d8ccc-129">A duração que o conector aguardará por uma resposta do aplicativo backend antes de fechar a conexão.</span><span class="sxs-lookup"><span data-stu-id="d8ccc-129">The duration the connector will wait for a response from the backend application before closing the connection.</span></span> <span data-ttu-id="d8ccc-130">Os valores possíveis `default`são `long`:.</span><span class="sxs-lookup"><span data-stu-id="d8ccc-130">Possible values are `default`, `long`.</span></span> <span data-ttu-id="d8ccc-131">Use `long` se o servidor levar mais de 60-75 segundos para responder às solicitações.</span><span class="sxs-lookup"><span data-stu-id="d8ccc-131">Use `long` if your server takes more than 60-75 seconds to respond to requests.</span></span> <span data-ttu-id="d8ccc-132">Além disso `long` , tente se você não consegue acessar o aplicativo e o status do erro é "tempo limite de backend".</span><span class="sxs-lookup"><span data-stu-id="d8ccc-132">Also try `long` if you are unable to access the application and the error status is "Backend Timeout".</span></span>|
|<span data-ttu-id="d8ccc-133">isTranslateHostHeaderEnabled</span><span class="sxs-lookup"><span data-stu-id="d8ccc-133">isTranslateHostHeaderEnabled</span></span>|<span data-ttu-id="d8ccc-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="d8ccc-134">Boolean</span></span>|<span data-ttu-id="d8ccc-135">Indica se o aplicativo deve traduzir URLs nos cabeçalhos de resposta.</span><span class="sxs-lookup"><span data-stu-id="d8ccc-135">Indicates if the application should translate urls in the reponse headers.</span></span> <span data-ttu-id="d8ccc-136">Isso inclui a configuração do site correto para cookies.</span><span class="sxs-lookup"><span data-stu-id="d8ccc-136">This includes setting the correct site for cookies.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d8ccc-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d8ccc-137">JSON representation</span></span>

<span data-ttu-id="d8ccc-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d8ccc-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishing"
}-->

```json
{
  "customDomainCertificate": "String",
  "externalAuthenticationType": "String",
  "externalUrl": "String",
  "internalUrl": "String",
  "isOnPremPublishingEnabled": true,
  "applicationServerTimeout": "String",
  "isTranslateHostHeaderEnabled": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2019-02-04 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesPublishing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
