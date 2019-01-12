---
title: Tipo de recurso configurationManagerClientEnabledFeatures
description: recursos habilitados pelo cliente do Gerenciador de Configurações
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dc1b994615c89b1a6e73785a5ebcdc85f0638953
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987588"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="9e428-103">Tipo de recurso configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="9e428-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="9e428-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9e428-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9e428-105">recursos habilitados pelo cliente do Gerenciador de Configurações</span><span class="sxs-lookup"><span data-stu-id="9e428-105">configuration Manager client enabled features</span></span>
## <a name="properties"></a><span data-ttu-id="9e428-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9e428-106">Properties</span></span>
|<span data-ttu-id="9e428-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e428-107">Property</span></span>|<span data-ttu-id="9e428-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e428-108">Type</span></span>|<span data-ttu-id="9e428-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e428-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e428-110">inventory</span><span class="sxs-lookup"><span data-stu-id="9e428-110">inventory</span></span>|<span data-ttu-id="9e428-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="9e428-111">Boolean</span></span>|<span data-ttu-id="9e428-112">Se o estoque é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="9e428-112">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="9e428-113">modernApps</span><span class="sxs-lookup"><span data-stu-id="9e428-113">modernApps</span></span>|<span data-ttu-id="9e428-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="9e428-114">Boolean</span></span>|<span data-ttu-id="9e428-115">Se o aplicativo moderno é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="9e428-115">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="9e428-116">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="9e428-116">resourceAccess</span></span>|<span data-ttu-id="9e428-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="9e428-117">Boolean</span></span>|<span data-ttu-id="9e428-118">Se o acesso ao recurso é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="9e428-118">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="9e428-119">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="9e428-119">deviceConfiguration</span></span>|<span data-ttu-id="9e428-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="9e428-120">Boolean</span></span>|<span data-ttu-id="9e428-121">Se a configuração do dispositivo é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="9e428-121">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="9e428-122">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="9e428-122">compliancePolicy</span></span>|<span data-ttu-id="9e428-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="9e428-123">Boolean</span></span>|<span data-ttu-id="9e428-124">Se a política de conformidade é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="9e428-124">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="9e428-125">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="9e428-125">windowsUpdateForBusiness</span></span>|<span data-ttu-id="9e428-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="9e428-126">Boolean</span></span>|<span data-ttu-id="9e428-127">Se o Windows Update para Empresas é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="9e428-127">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e428-128">Relações</span><span class="sxs-lookup"><span data-stu-id="9e428-128">Relationships</span></span>
<span data-ttu-id="9e428-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9e428-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9e428-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9e428-130">JSON Representation</span></span>
<span data-ttu-id="9e428-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9e428-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientEnabledFeatures",
  "inventory": true,
  "modernApps": true,
  "resourceAccess": true,
  "deviceConfiguration": true,
  "compliancePolicy": true,
  "windowsUpdateForBusiness": true
}
```



