---
title: tipo de recurso de onPremisesPublishing
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 8dba505347fc12d3c4a8521ebe32551d738dc4a2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037022"
---
# <a name="onpremisespublishing-resource-type"></a><span data-ttu-id="0f50d-103">tipo de recurso de onPremisesPublishing</span><span class="sxs-lookup"><span data-stu-id="0f50d-103">onPremisesPublishing resource type</span></span>

> <span data-ttu-id="0f50d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0f50d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f50d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0f50d-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="0f50d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0f50d-106">Properties</span></span>
| <span data-ttu-id="0f50d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f50d-107">Property</span></span>     | <span data-ttu-id="0f50d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f50d-108">Type</span></span>   |<span data-ttu-id="0f50d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f50d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f50d-110">customDomainCertificate</span><span class="sxs-lookup"><span data-stu-id="0f50d-110">customDomainCertificate</span></span>|<span data-ttu-id="0f50d-111">String</span><span class="sxs-lookup"><span data-stu-id="0f50d-111">String</span></span>|<span data-ttu-id="0f50d-112">Detalhes do certificado associado ao aplicativo quando um domínio personalizado está em uso.</span><span class="sxs-lookup"><span data-stu-id="0f50d-112">Details of the certificate associated with the applicaiton when a custom domain is in use.</span></span> <span data-ttu-id="0f50d-113">Nulo ao usar o domínio padrão.</span><span class="sxs-lookup"><span data-stu-id="0f50d-113">Null when using the default domain.</span></span>|
|<span data-ttu-id="0f50d-114">externalAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="0f50d-114">externalAuthenticationType</span></span>|<span data-ttu-id="0f50d-115">String</span><span class="sxs-lookup"><span data-stu-id="0f50d-115">String</span></span>|<span data-ttu-id="0f50d-116">Detalha a configuração de pré-autenticação para os aplicativo os valores possíveis são: `passthru`, `aadPreAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="0f50d-116">Details the pre-authentication setting for the application Possible values are: `passthru`, `aadPreAuthentication`.</span></span>|
|<span data-ttu-id="0f50d-117">externalUrl</span><span class="sxs-lookup"><span data-stu-id="0f50d-117">externalUrl</span></span>|<span data-ttu-id="0f50d-118">String</span><span class="sxs-lookup"><span data-stu-id="0f50d-118">String</span></span>|<span data-ttu-id="0f50d-119">A url externa publicada para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f50d-119">The published external url for the application.</span></span> <span data-ttu-id="0f50d-120">Por exemplohttps://intranet-contoso.msappproxy.net/</span><span class="sxs-lookup"><span data-stu-id="0f50d-120">For example https://intranet-contoso.msappproxy.net/</span></span>  |
|<span data-ttu-id="0f50d-121">internalUrl</span><span class="sxs-lookup"><span data-stu-id="0f50d-121">internalUrl</span></span>|<span data-ttu-id="0f50d-122">String</span><span class="sxs-lookup"><span data-stu-id="0f50d-122">String</span></span>|<span data-ttu-id="0f50d-123">A url interna do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f50d-123">The internal url of the application.</span></span> <span data-ttu-id="0f50d-124">Por exemplohttps://intranet/</span><span class="sxs-lookup"><span data-stu-id="0f50d-124">For example https://intranet/</span></span> |
|<span data-ttu-id="0f50d-125">isOnPremPublishingEnabled</span><span class="sxs-lookup"><span data-stu-id="0f50d-125">isOnPremPublishingEnabled</span></span>|<span data-ttu-id="0f50d-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="0f50d-126">Boolean</span></span>|<span data-ttu-id="0f50d-127">Indica se o aplicativo atualmente está sendo publicado ou não.</span><span class="sxs-lookup"><span data-stu-id="0f50d-127">Indicates if the application is currently being published or not.</span></span>|
|<span data-ttu-id="0f50d-128">applicationServerTimeout</span><span class="sxs-lookup"><span data-stu-id="0f50d-128">applicationServerTimeout</span></span>|<span data-ttu-id="0f50d-129">String</span><span class="sxs-lookup"><span data-stu-id="0f50d-129">String</span></span>|<span data-ttu-id="0f50d-130">A duração o conector aguardará uma resposta do aplicativo back-end antes de fechar a conexão.</span><span class="sxs-lookup"><span data-stu-id="0f50d-130">The duration the connector will wait for a response from the backend application before closing the connection.</span></span> <span data-ttu-id="0f50d-131">Os valores possíveis são `default`, `long`.</span><span class="sxs-lookup"><span data-stu-id="0f50d-131">Possible values are `default`, `long`.</span></span> <span data-ttu-id="0f50d-132">Uso `long` se seu servidor demorar mais de 75-60 segundos para responder às solicitações.</span><span class="sxs-lookup"><span data-stu-id="0f50d-132">Use `long` if your server takes more than 60-75 seconds to respond to requests.</span></span> <span data-ttu-id="0f50d-133">Além disso, experimente `long` se não for possível acessar o aplicativo e o status de erro é "Backend Timeout".</span><span class="sxs-lookup"><span data-stu-id="0f50d-133">Also try `long` if you are unable to access the application and the error status is "Backend Timeout".</span></span>|
|<span data-ttu-id="0f50d-134">isTranslateHostHeaderEnabled</span><span class="sxs-lookup"><span data-stu-id="0f50d-134">isTranslateHostHeaderEnabled</span></span>|<span data-ttu-id="0f50d-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="0f50d-135">Boolean</span></span>|<span data-ttu-id="0f50d-136">Indica se o aplicativo deve traduzir urls em cabeçalhos de resposta.</span><span class="sxs-lookup"><span data-stu-id="0f50d-136">Indicates if the application should translate urls in the reponse headers.</span></span> <span data-ttu-id="0f50d-137">Isso inclui a definição de site correto para os cookies.</span><span class="sxs-lookup"><span data-stu-id="0f50d-137">This includes setting the correct site for cookies.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0f50d-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0f50d-138">JSON representation</span></span>

<span data-ttu-id="0f50d-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0f50d-139">Here is a JSON representation of the resource.</span></span>

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
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesPublishing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
