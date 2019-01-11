---
title: tipo de recurso de implicitGrantSettings
description: Especifica se esse aplicativo web pode solicitar tokens usando o fluxo de implícita OAuth 2.0. Propriedades separadas estão disponíveis para solicitar tokens de acesso e a ID como parte do fluxo de implícita. Para ativar o fluxo implícito, pelo menos uma das propriedades a seguir deve ser definida como true.
localization_priority: Normal
ms.openlocfilehash: 93a54ac0c0e4c6c32ebb99c9747d44d75f98af07
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834262"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="20d4d-105">tipo de recurso de implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="20d4d-105">implicitGrantSettings resource type</span></span>

> <span data-ttu-id="20d4d-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="20d4d-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="20d4d-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="20d4d-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="20d4d-108">Especifica se esse aplicativo web pode solicitar tokens usando o fluxo de implícita OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="20d4d-108">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="20d4d-109">Propriedades separadas estão disponíveis para solicitar tokens de acesso e a ID como parte do fluxo de implícita.</span><span class="sxs-lookup"><span data-stu-id="20d4d-109">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="20d4d-110">Para ativar o fluxo implícito, pelo menos uma das propriedades a seguir deve ser definida como true.</span><span class="sxs-lookup"><span data-stu-id="20d4d-110">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="20d4d-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="20d4d-111">Properties</span></span>

| <span data-ttu-id="20d4d-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20d4d-112">Property</span></span> | <span data-ttu-id="20d4d-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="20d4d-113">Type</span></span> | <span data-ttu-id="20d4d-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="20d4d-114">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="20d4d-115">enableIdTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="20d4d-115">enableIdTokenIssuance</span></span>| <span data-ttu-id="20d4d-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="20d4d-116">Boolean</span></span> | <span data-ttu-id="20d4d-117">Especifica se esse aplicativo web pode solicitar um token de ID usando o fluxo de implícita OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="20d4d-117">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="20d4d-118">enableAccessTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="20d4d-118">enableAccessTokenIssuance</span></span>| <span data-ttu-id="20d4d-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="20d4d-119">Boolean</span></span> | <span data-ttu-id="20d4d-120">Especifica se esse aplicativo web pode solicitar um token de acesso usando o fluxo de implícita OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="20d4d-120">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="20d4d-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="20d4d-121">JSON representation</span></span>
<span data-ttu-id="20d4d-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="20d4d-122">Here is a JSON representation of the resource.</span></span>

```json
{
  "enableIdTokenIssuance": "Boolean",
  "enableAccessTokenIssuance": "Boolean"
}

```
