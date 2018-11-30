---
title: Tipo de recurso configurationManagerClientEnabledFeatures
description: recursos habilitados pelo cliente do Gerenciador de Configurações
ms.openlocfilehash: 60d0e9e78bc4b641bb1f9ee0d61cc09744500424
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034503"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="79315-103">Tipo de recurso configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="79315-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="79315-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="79315-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79315-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="79315-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="79315-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="79315-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="79315-107">recursos habilitados pelo cliente do Gerenciador de Configurações</span><span class="sxs-lookup"><span data-stu-id="79315-107">configuration Manager client enabled features</span></span>
## <a name="properties"></a><span data-ttu-id="79315-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="79315-108">Properties</span></span>
|<span data-ttu-id="79315-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79315-109">Property</span></span>|<span data-ttu-id="79315-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="79315-110">Type</span></span>|<span data-ttu-id="79315-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="79315-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79315-112">inventory</span><span class="sxs-lookup"><span data-stu-id="79315-112">inventory</span></span>|<span data-ttu-id="79315-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="79315-113">Boolean</span></span>|<span data-ttu-id="79315-114">Se o estoque é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="79315-114">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="79315-115">modernApps</span><span class="sxs-lookup"><span data-stu-id="79315-115">modernApps</span></span>|<span data-ttu-id="79315-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="79315-116">Boolean</span></span>|<span data-ttu-id="79315-117">Se o aplicativo moderno é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="79315-117">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="79315-118">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="79315-118">resourceAccess</span></span>|<span data-ttu-id="79315-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="79315-119">Boolean</span></span>|<span data-ttu-id="79315-120">Se o acesso ao recurso é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="79315-120">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="79315-121">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="79315-121">deviceConfiguration</span></span>|<span data-ttu-id="79315-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="79315-122">Boolean</span></span>|<span data-ttu-id="79315-123">Se a configuração do dispositivo é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="79315-123">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="79315-124">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="79315-124">compliancePolicy</span></span>|<span data-ttu-id="79315-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="79315-125">Boolean</span></span>|<span data-ttu-id="79315-126">Se a política de conformidade é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="79315-126">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="79315-127">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="79315-127">windowsUpdateForBusiness</span></span>|<span data-ttu-id="79315-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="79315-128">Boolean</span></span>|<span data-ttu-id="79315-129">Se o Windows Update para Empresas é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="79315-129">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="79315-130">Relações</span><span class="sxs-lookup"><span data-stu-id="79315-130">Relationships</span></span>
<span data-ttu-id="79315-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="79315-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="79315-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="79315-132">JSON Representation</span></span>
<span data-ttu-id="79315-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="79315-133">Here is a JSON representation of the resource.</span></span>
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





