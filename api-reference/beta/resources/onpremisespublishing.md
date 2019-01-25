---
title: tipo de recurso de onPremisesPublishing
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: fd216d52ba212e739f1d7c087a99a4379682010e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508178"
---
# <a name="onpremisespublishing-resource-type"></a><span data-ttu-id="fb812-103">tipo de recurso de onPremisesPublishing</span><span class="sxs-lookup"><span data-stu-id="fb812-103">onPremisesPublishing resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="fb812-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fb812-104">Properties</span></span>
| <span data-ttu-id="fb812-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb812-105">Property</span></span>     | <span data-ttu-id="fb812-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb812-106">Type</span></span>   |<span data-ttu-id="fb812-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb812-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb812-108">customDomainCertificate</span><span class="sxs-lookup"><span data-stu-id="fb812-108">customDomainCertificate</span></span>|<span data-ttu-id="fb812-109">String</span><span class="sxs-lookup"><span data-stu-id="fb812-109">String</span></span>|<span data-ttu-id="fb812-110">Detalhes do certificado associado ao aplicativo quando um domínio personalizado está em uso.</span><span class="sxs-lookup"><span data-stu-id="fb812-110">Details of the certificate associated with the applicaiton when a custom domain is in use.</span></span> <span data-ttu-id="fb812-111">Nulo ao usar o domínio padrão.</span><span class="sxs-lookup"><span data-stu-id="fb812-111">Null when using the default domain.</span></span>|
|<span data-ttu-id="fb812-112">externalAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="fb812-112">externalAuthenticationType</span></span>|<span data-ttu-id="fb812-113">String</span><span class="sxs-lookup"><span data-stu-id="fb812-113">String</span></span>|<span data-ttu-id="fb812-114">Detalha a configuração de pré-autenticação para os aplicativo os valores possíveis são: `passthru`, `aadPreAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="fb812-114">Details the pre-authentication setting for the application Possible values are: `passthru`, `aadPreAuthentication`.</span></span>|
|<span data-ttu-id="fb812-115">externalUrl</span><span class="sxs-lookup"><span data-stu-id="fb812-115">externalUrl</span></span>|<span data-ttu-id="fb812-116">String</span><span class="sxs-lookup"><span data-stu-id="fb812-116">String</span></span>|<span data-ttu-id="fb812-117">A url externa publicada para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb812-117">The published external url for the application.</span></span> <span data-ttu-id="fb812-118">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="fb812-118">For example https://intranet-contoso.msappproxy.net/</span></span>  |
|<span data-ttu-id="fb812-119">internalUrl</span><span class="sxs-lookup"><span data-stu-id="fb812-119">internalUrl</span></span>|<span data-ttu-id="fb812-120">String</span><span class="sxs-lookup"><span data-stu-id="fb812-120">String</span></span>|<span data-ttu-id="fb812-121">A url interna do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb812-121">The internal url of the application.</span></span> <span data-ttu-id="fb812-122">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="fb812-122">For example https://intranet/</span></span> |
|<span data-ttu-id="fb812-123">isOnPremPublishingEnabled</span><span class="sxs-lookup"><span data-stu-id="fb812-123">isOnPremPublishingEnabled</span></span>|<span data-ttu-id="fb812-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="fb812-124">Boolean</span></span>|<span data-ttu-id="fb812-125">Indica se o aplicativo atualmente está sendo publicado ou não.</span><span class="sxs-lookup"><span data-stu-id="fb812-125">Indicates if the application is currently being published or not.</span></span>|
|<span data-ttu-id="fb812-126">applicationServerTimeout</span><span class="sxs-lookup"><span data-stu-id="fb812-126">applicationServerTimeout</span></span>|<span data-ttu-id="fb812-127">String</span><span class="sxs-lookup"><span data-stu-id="fb812-127">String</span></span>|<span data-ttu-id="fb812-128">A duração o conector aguardará uma resposta do aplicativo back-end antes de fechar a conexão.</span><span class="sxs-lookup"><span data-stu-id="fb812-128">The duration the connector will wait for a response from the backend application before closing the connection.</span></span> <span data-ttu-id="fb812-129">Os valores possíveis são: `default` e `long`.</span><span class="sxs-lookup"><span data-stu-id="fb812-129">Possible values are `default`, `long`.</span></span> <span data-ttu-id="fb812-130">Uso `long` se seu servidor demorar mais de 75-60 segundos para responder às solicitações.</span><span class="sxs-lookup"><span data-stu-id="fb812-130">Use `long` if your server takes more than 60-75 seconds to respond to requests.</span></span> <span data-ttu-id="fb812-131">Além disso, experimente `long` se não for possível acessar o aplicativo e o status de erro é "Backend Timeout".</span><span class="sxs-lookup"><span data-stu-id="fb812-131">Also try `long` if you are unable to access the application and the error status is "Backend Timeout".</span></span>|
|<span data-ttu-id="fb812-132">isTranslateHostHeaderEnabled</span><span class="sxs-lookup"><span data-stu-id="fb812-132">isTranslateHostHeaderEnabled</span></span>|<span data-ttu-id="fb812-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="fb812-133">Boolean</span></span>|<span data-ttu-id="fb812-134">Indica se o aplicativo deve traduzir urls em cabeçalhos de resposta.</span><span class="sxs-lookup"><span data-stu-id="fb812-134">Indicates if the application should translate urls in the reponse headers.</span></span> <span data-ttu-id="fb812-135">Isso inclui a definição de site correto para os cookies.</span><span class="sxs-lookup"><span data-stu-id="fb812-135">This includes setting the correct site for cookies.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fb812-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fb812-136">JSON representation</span></span>

<span data-ttu-id="fb812-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fb812-137">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesPublishing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onpremisespublishing.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
