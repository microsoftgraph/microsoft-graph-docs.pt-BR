---
title: Tipo de recurso registrationEnforcement
description: Impor o registro no momento da inscrição.
author: mjsantani
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 86d3e974ccfebdf0011c9c19f881096e3fb2ba40
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682856"
---
# <a name="registrationenforcement-resource-type"></a><span data-ttu-id="b5a7f-103">Tipo de recurso registrationEnforcement</span><span class="sxs-lookup"><span data-stu-id="b5a7f-103">registrationEnforcement resource type</span></span>

<span data-ttu-id="b5a7f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5a7f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5a7f-105">Impor o registro no momento da inscrição.</span><span class="sxs-lookup"><span data-stu-id="b5a7f-105">Enforce registration at sign-in time.</span></span> <span data-ttu-id="b5a7f-106">Atualmente, isso só pode ser usado para lembrar os usuários de configurar métodos de autenticação direcionada (Microsoft Authenticator) usando a "authenticationMethodsRegistrationCampaign".</span><span class="sxs-lookup"><span data-stu-id="b5a7f-106">This can currently only be used to remind users to set up targeted authentication methods (Microsoft Authenticator) using the 'authenticationMethodsRegistrationCampaign\`.</span></span>

## <a name="properties"></a><span data-ttu-id="b5a7f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b5a7f-107">Properties</span></span>
|<span data-ttu-id="b5a7f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b5a7f-108">Property</span></span>|<span data-ttu-id="b5a7f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5a7f-109">Type</span></span>|<span data-ttu-id="b5a7f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5a7f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5a7f-111">authenticationMethodsRegistrationCampaign</span><span class="sxs-lookup"><span data-stu-id="b5a7f-111">authenticationMethodsRegistrationCampaign</span></span>|[<span data-ttu-id="b5a7f-112">authenticationMethodsRegistrationCampaign</span><span class="sxs-lookup"><span data-stu-id="b5a7f-112">authenticationMethodsRegistrationCampaign</span></span>](../resources/authenticationmethodsregistrationcampaign.md)|<span data-ttu-id="b5a7f-113">Execute campanhas para lembrar os usuários de configurar métodos de autenticação direcionada.</span><span class="sxs-lookup"><span data-stu-id="b5a7f-113">Run campaigns to remind users to setup targeted authentication methods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5a7f-114">Relações</span><span class="sxs-lookup"><span data-stu-id="b5a7f-114">Relationships</span></span>
<span data-ttu-id="b5a7f-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b5a7f-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b5a7f-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b5a7f-116">JSON representation</span></span>
<span data-ttu-id="b5a7f-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b5a7f-117">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.registrationEnforcement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.registrationEnforcement",
  "authenticationMethodsRegistrationCampaign": {
    "@odata.type": "microsoft.graph.authenticationMethodsRegistrationCampaign"
  }
}
```
