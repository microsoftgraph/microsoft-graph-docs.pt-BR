---
title: Tipo de recurso configurationManagerClientEnabledFeatures
description: recursos habilitados pelo cliente do Gerenciador de Configurações
author: tfitzmac
ms.openlocfilehash: fe975f2e8d537d1231a89eb9f2a44cdd8258fd1a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325141"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="e2a6b-103">Tipo de recurso configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="e2a6b-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="e2a6b-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e2a6b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e2a6b-105">recursos habilitados pelo cliente do Gerenciador de Configurações</span><span class="sxs-lookup"><span data-stu-id="e2a6b-105">configuration Manager client enabled features</span></span>
## <a name="properties"></a><span data-ttu-id="e2a6b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e2a6b-106">Properties</span></span>
|<span data-ttu-id="e2a6b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2a6b-107">Property</span></span>|<span data-ttu-id="e2a6b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2a6b-108">Type</span></span>|<span data-ttu-id="e2a6b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2a6b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2a6b-110">inventory</span><span class="sxs-lookup"><span data-stu-id="e2a6b-110">inventory</span></span>|<span data-ttu-id="e2a6b-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2a6b-111">Boolean</span></span>|<span data-ttu-id="e2a6b-112">Se o estoque é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="e2a6b-112">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="e2a6b-113">modernApps</span><span class="sxs-lookup"><span data-stu-id="e2a6b-113">modernApps</span></span>|<span data-ttu-id="e2a6b-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2a6b-114">Boolean</span></span>|<span data-ttu-id="e2a6b-115">Se o aplicativo moderno é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="e2a6b-115">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="e2a6b-116">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="e2a6b-116">resourceAccess</span></span>|<span data-ttu-id="e2a6b-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2a6b-117">Boolean</span></span>|<span data-ttu-id="e2a6b-118">Se o acesso ao recurso é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="e2a6b-118">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="e2a6b-119">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="e2a6b-119">deviceConfiguration</span></span>|<span data-ttu-id="e2a6b-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2a6b-120">Boolean</span></span>|<span data-ttu-id="e2a6b-121">Se a configuração do dispositivo é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="e2a6b-121">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="e2a6b-122">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="e2a6b-122">compliancePolicy</span></span>|<span data-ttu-id="e2a6b-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2a6b-123">Boolean</span></span>|<span data-ttu-id="e2a6b-124">Se a política de conformidade é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="e2a6b-124">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="e2a6b-125">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="e2a6b-125">windowsUpdateForBusiness</span></span>|<span data-ttu-id="e2a6b-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2a6b-126">Boolean</span></span>|<span data-ttu-id="e2a6b-127">Se o Windows Update para Empresas é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="e2a6b-127">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2a6b-128">Relações</span><span class="sxs-lookup"><span data-stu-id="e2a6b-128">Relationships</span></span>
<span data-ttu-id="e2a6b-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e2a6b-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e2a6b-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e2a6b-130">JSON Representation</span></span>
<span data-ttu-id="e2a6b-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e2a6b-131">Here is a JSON representation of the resource.</span></span>
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



