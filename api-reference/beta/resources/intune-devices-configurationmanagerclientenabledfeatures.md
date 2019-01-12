---
title: Tipo de recurso configurationManagerClientEnabledFeatures
description: recursos habilitados pelo cliente do Gerenciador de Configurações
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 07b143a8d61335c44c83d1d88b9a67d2d3c2e4dc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962083"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="beb8c-103">Tipo de recurso configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="beb8c-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="beb8c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="beb8c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="beb8c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="beb8c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="beb8c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="beb8c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="beb8c-107">recursos habilitados pelo cliente do Gerenciador de Configurações</span><span class="sxs-lookup"><span data-stu-id="beb8c-107">configuration Manager client enabled features</span></span>
## <a name="properties"></a><span data-ttu-id="beb8c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="beb8c-108">Properties</span></span>
|<span data-ttu-id="beb8c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="beb8c-109">Property</span></span>|<span data-ttu-id="beb8c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="beb8c-110">Type</span></span>|<span data-ttu-id="beb8c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="beb8c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="beb8c-112">inventory</span><span class="sxs-lookup"><span data-stu-id="beb8c-112">inventory</span></span>|<span data-ttu-id="beb8c-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="beb8c-113">Boolean</span></span>|<span data-ttu-id="beb8c-114">Se o estoque é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="beb8c-114">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="beb8c-115">modernApps</span><span class="sxs-lookup"><span data-stu-id="beb8c-115">modernApps</span></span>|<span data-ttu-id="beb8c-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="beb8c-116">Boolean</span></span>|<span data-ttu-id="beb8c-117">Se o aplicativo moderno é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="beb8c-117">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="beb8c-118">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="beb8c-118">resourceAccess</span></span>|<span data-ttu-id="beb8c-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="beb8c-119">Boolean</span></span>|<span data-ttu-id="beb8c-120">Se o acesso ao recurso é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="beb8c-120">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="beb8c-121">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="beb8c-121">deviceConfiguration</span></span>|<span data-ttu-id="beb8c-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="beb8c-122">Boolean</span></span>|<span data-ttu-id="beb8c-123">Se a configuração do dispositivo é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="beb8c-123">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="beb8c-124">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="beb8c-124">compliancePolicy</span></span>|<span data-ttu-id="beb8c-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="beb8c-125">Boolean</span></span>|<span data-ttu-id="beb8c-126">Se a política de conformidade é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="beb8c-126">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="beb8c-127">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="beb8c-127">windowsUpdateForBusiness</span></span>|<span data-ttu-id="beb8c-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="beb8c-128">Boolean</span></span>|<span data-ttu-id="beb8c-129">Se o Windows Update para Empresas é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="beb8c-129">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="beb8c-130">Relações</span><span class="sxs-lookup"><span data-stu-id="beb8c-130">Relationships</span></span>
<span data-ttu-id="beb8c-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="beb8c-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="beb8c-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="beb8c-132">JSON Representation</span></span>
<span data-ttu-id="beb8c-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="beb8c-133">Here is a JSON representation of the resource.</span></span>
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





