---
title: tipo de recurso onPremisesPublishing
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: db81ef2c61142edb0d3ca58a67b34c7da34e71f9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522211"
---
# <a name="onpremisespublishing-resource-type"></a><span data-ttu-id="5ba41-103">tipo de recurso onPremisesPublishing</span><span class="sxs-lookup"><span data-stu-id="5ba41-103">onPremisesPublishing resource type</span></span>

<span data-ttu-id="5ba41-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5ba41-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ba41-105">Um objeto **onPremisesPublishing** representa o conjunto de propriedades para publicar o [aplicativo](application.md)local.</span><span class="sxs-lookup"><span data-stu-id="5ba41-105">An **onPremisesPublishing** object represents the set of properties for publishing of on-premises [application](application.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5ba41-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5ba41-106">Properties</span></span>

| <span data-ttu-id="5ba41-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ba41-107">Property</span></span>|<span data-ttu-id="5ba41-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ba41-108">Type</span></span>|<span data-ttu-id="5ba41-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ba41-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ba41-110">customDomainCertificate</span><span class="sxs-lookup"><span data-stu-id="5ba41-110">customDomainCertificate</span></span>|<span data-ttu-id="5ba41-111">String</span><span class="sxs-lookup"><span data-stu-id="5ba41-111">String</span></span>|<span data-ttu-id="5ba41-112">Detalhes do certificado associado ao aplicativo quando um domínio personalizado está em uso.</span><span class="sxs-lookup"><span data-stu-id="5ba41-112">Details of the certificate associated with the applicaiton when a custom domain is in use.</span></span> <span data-ttu-id="5ba41-113">Nulo ao usar o domínio padrão.</span><span class="sxs-lookup"><span data-stu-id="5ba41-113">Null when using the default domain.</span></span>|
|<span data-ttu-id="5ba41-114">externalAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="5ba41-114">externalAuthenticationType</span></span>|<span data-ttu-id="5ba41-115">String</span><span class="sxs-lookup"><span data-stu-id="5ba41-115">String</span></span>|<span data-ttu-id="5ba41-116">Detalhes a configuração de pré-autenticação para o aplicativo os valores possíveis são: `passthru`, `aadPreAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="5ba41-116">Details the pre-authentication setting for the application Possible values are: `passthru`, `aadPreAuthentication`.</span></span>|
|<span data-ttu-id="5ba41-117">externalUrl</span><span class="sxs-lookup"><span data-stu-id="5ba41-117">externalUrl</span></span>|<span data-ttu-id="5ba41-118">String</span><span class="sxs-lookup"><span data-stu-id="5ba41-118">String</span></span>|<span data-ttu-id="5ba41-119">A URL externa publicada para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5ba41-119">The published external url for the application.</span></span> <span data-ttu-id="5ba41-120">Por exemplohttps://intranet-contoso.msappproxy.net/</span><span class="sxs-lookup"><span data-stu-id="5ba41-120">For example https://intranet-contoso.msappproxy.net/</span></span>  |
|<span data-ttu-id="5ba41-121">internalUrl</span><span class="sxs-lookup"><span data-stu-id="5ba41-121">internalUrl</span></span>|<span data-ttu-id="5ba41-122">String</span><span class="sxs-lookup"><span data-stu-id="5ba41-122">String</span></span>|<span data-ttu-id="5ba41-123">A URL interna do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5ba41-123">The internal url of the application.</span></span> <span data-ttu-id="5ba41-124">Por exemplohttps://intranet/</span><span class="sxs-lookup"><span data-stu-id="5ba41-124">For example https://intranet/</span></span> |
|<span data-ttu-id="5ba41-125">isOnPremPublishingEnabled</span><span class="sxs-lookup"><span data-stu-id="5ba41-125">isOnPremPublishingEnabled</span></span>|<span data-ttu-id="5ba41-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ba41-126">Boolean</span></span>|<span data-ttu-id="5ba41-127">Indica se o aplicativo está sendo publicado ou não no momento.</span><span class="sxs-lookup"><span data-stu-id="5ba41-127">Indicates if the application is currently being published or not.</span></span>|
|<span data-ttu-id="5ba41-128">applicationServerTimeout</span><span class="sxs-lookup"><span data-stu-id="5ba41-128">applicationServerTimeout</span></span>|<span data-ttu-id="5ba41-129">String</span><span class="sxs-lookup"><span data-stu-id="5ba41-129">String</span></span>|<span data-ttu-id="5ba41-130">A duração que o conector aguardará por uma resposta do aplicativo backend antes de fechar a conexão.</span><span class="sxs-lookup"><span data-stu-id="5ba41-130">The duration the connector will wait for a response from the backend application before closing the connection.</span></span> <span data-ttu-id="5ba41-131">Os valores possíveis `default`são `long`:.</span><span class="sxs-lookup"><span data-stu-id="5ba41-131">Possible values are `default`, `long`.</span></span> <span data-ttu-id="5ba41-132">Use `long` se o servidor levar mais de 60-75 segundos para responder às solicitações.</span><span class="sxs-lookup"><span data-stu-id="5ba41-132">Use `long` if your server takes more than 60-75 seconds to respond to requests.</span></span> <span data-ttu-id="5ba41-133">Além disso `long` , tente se você não consegue acessar o aplicativo e o status do erro é "tempo limite de backend".</span><span class="sxs-lookup"><span data-stu-id="5ba41-133">Also try `long` if you are unable to access the application and the error status is "Backend Timeout".</span></span>|
|<span data-ttu-id="5ba41-134">isTranslateHostHeaderEnabled</span><span class="sxs-lookup"><span data-stu-id="5ba41-134">isTranslateHostHeaderEnabled</span></span>|<span data-ttu-id="5ba41-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ba41-135">Boolean</span></span>|<span data-ttu-id="5ba41-136">Indica se o aplicativo deve traduzir URLs nos cabeçalhos de resposta.</span><span class="sxs-lookup"><span data-stu-id="5ba41-136">Indicates if the application should translate urls in the reponse headers.</span></span> <span data-ttu-id="5ba41-137">Isso inclui a configuração do site correto para cookies.</span><span class="sxs-lookup"><span data-stu-id="5ba41-137">This includes setting the correct site for cookies.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5ba41-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5ba41-138">JSON representation</span></span>

<span data-ttu-id="5ba41-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5ba41-139">Here is a JSON representation of the resource.</span></span>

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
