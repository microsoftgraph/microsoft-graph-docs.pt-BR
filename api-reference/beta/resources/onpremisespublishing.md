---
title: tipo de recurso onPremisesPublishing
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: fd216d52ba212e739f1d7c087a99a4379682010e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568855"
---
# <a name="onpremisespublishing-resource-type"></a><span data-ttu-id="32e68-103">tipo de recurso onPremisesPublishing</span><span class="sxs-lookup"><span data-stu-id="32e68-103">onPremisesPublishing resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="32e68-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="32e68-104">Properties</span></span>
| <span data-ttu-id="32e68-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32e68-105">Property</span></span>     | <span data-ttu-id="32e68-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="32e68-106">Type</span></span>   |<span data-ttu-id="32e68-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="32e68-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32e68-108">customDomainCertificate</span><span class="sxs-lookup"><span data-stu-id="32e68-108">customDomainCertificate</span></span>|<span data-ttu-id="32e68-109">String</span><span class="sxs-lookup"><span data-stu-id="32e68-109">String</span></span>|<span data-ttu-id="32e68-110">Detalhes do certificado associado ao aplicativo quando um domínio personalizado está em uso.</span><span class="sxs-lookup"><span data-stu-id="32e68-110">Details of the certificate associated with the applicaiton when a custom domain is in use.</span></span> <span data-ttu-id="32e68-111">Nulo ao usar o domínio padrão.</span><span class="sxs-lookup"><span data-stu-id="32e68-111">Null when using the default domain.</span></span>|
|<span data-ttu-id="32e68-112">externalAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="32e68-112">externalAuthenticationType</span></span>|<span data-ttu-id="32e68-113">String</span><span class="sxs-lookup"><span data-stu-id="32e68-113">String</span></span>|<span data-ttu-id="32e68-114">Detalhes a configuração de pré-autenticação para o aplicativo os valores possíveis são: `passthru`, `aadPreAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="32e68-114">Details the pre-authentication setting for the application Possible values are: `passthru`, `aadPreAuthentication`.</span></span>|
|<span data-ttu-id="32e68-115">externalUrl</span><span class="sxs-lookup"><span data-stu-id="32e68-115">externalUrl</span></span>|<span data-ttu-id="32e68-116">String</span><span class="sxs-lookup"><span data-stu-id="32e68-116">String</span></span>|<span data-ttu-id="32e68-117">A URL externa publicada para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="32e68-117">The published external url for the application.</span></span> <span data-ttu-id="32e68-118">Por exemplohttps://intranet-contoso.msappproxy.net/</span><span class="sxs-lookup"><span data-stu-id="32e68-118">For example https://intranet-contoso.msappproxy.net/</span></span>  |
|<span data-ttu-id="32e68-119">internalUrl</span><span class="sxs-lookup"><span data-stu-id="32e68-119">internalUrl</span></span>|<span data-ttu-id="32e68-120">String</span><span class="sxs-lookup"><span data-stu-id="32e68-120">String</span></span>|<span data-ttu-id="32e68-121">A URL interna do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="32e68-121">The internal url of the application.</span></span> <span data-ttu-id="32e68-122">Por exemplohttps://intranet/</span><span class="sxs-lookup"><span data-stu-id="32e68-122">For example https://intranet/</span></span> |
|<span data-ttu-id="32e68-123">isOnPremPublishingEnabled</span><span class="sxs-lookup"><span data-stu-id="32e68-123">isOnPremPublishingEnabled</span></span>|<span data-ttu-id="32e68-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="32e68-124">Boolean</span></span>|<span data-ttu-id="32e68-125">Indica se o aplicativo está sendo publicado ou não no momento.</span><span class="sxs-lookup"><span data-stu-id="32e68-125">Indicates if the application is currently being published or not.</span></span>|
|<span data-ttu-id="32e68-126">applicationServerTimeout</span><span class="sxs-lookup"><span data-stu-id="32e68-126">applicationServerTimeout</span></span>|<span data-ttu-id="32e68-127">String</span><span class="sxs-lookup"><span data-stu-id="32e68-127">String</span></span>|<span data-ttu-id="32e68-128">A duração que o conector aguardará por uma resposta do aplicativo backend antes de fechar a conexão.</span><span class="sxs-lookup"><span data-stu-id="32e68-128">The duration the connector will wait for a response from the backend application before closing the connection.</span></span> <span data-ttu-id="32e68-129">Os valores possíveis `default`são `long`:.</span><span class="sxs-lookup"><span data-stu-id="32e68-129">Possible values are `default`, `long`.</span></span> <span data-ttu-id="32e68-130">Use `long` se o servidor levar mais de 60-75 segundos para responder às solicitações.</span><span class="sxs-lookup"><span data-stu-id="32e68-130">Use `long` if your server takes more than 60-75 seconds to respond to requests.</span></span> <span data-ttu-id="32e68-131">Além disso `long` , tente se você não consegue acessar o aplicativo e o status do erro é "tempo limite de backend".</span><span class="sxs-lookup"><span data-stu-id="32e68-131">Also try `long` if you are unable to access the application and the error status is "Backend Timeout".</span></span>|
|<span data-ttu-id="32e68-132">isTranslateHostHeaderEnabled</span><span class="sxs-lookup"><span data-stu-id="32e68-132">isTranslateHostHeaderEnabled</span></span>|<span data-ttu-id="32e68-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="32e68-133">Boolean</span></span>|<span data-ttu-id="32e68-134">Indica se o aplicativo deve traduzir URLs nos cabeçalhos de resposta.</span><span class="sxs-lookup"><span data-stu-id="32e68-134">Indicates if the application should translate urls in the reponse headers.</span></span> <span data-ttu-id="32e68-135">Isso inclui a configuração do site correto para cookies.</span><span class="sxs-lookup"><span data-stu-id="32e68-135">This includes setting the correct site for cookies.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="32e68-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="32e68-136">JSON representation</span></span>

<span data-ttu-id="32e68-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="32e68-137">Here is a JSON representation of the resource.</span></span>

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
