---
title: Tipo de recurso configurationManagerClientEnabledFeatures
description: recursos habilitados pelo cliente do Gerenciador de Configurações
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 91ffd0180660b33e9ead5210f9b23870af18e29a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264418"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="d5491-103">Tipo de recurso configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="d5491-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="d5491-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d5491-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5491-105">recursos habilitados pelo cliente do Gerenciador de Configurações</span><span class="sxs-lookup"><span data-stu-id="d5491-105">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="d5491-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d5491-106">Properties</span></span>
|<span data-ttu-id="d5491-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5491-107">Property</span></span>|<span data-ttu-id="d5491-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5491-108">Type</span></span>|<span data-ttu-id="d5491-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5491-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5491-110">inventory</span><span class="sxs-lookup"><span data-stu-id="d5491-110">inventory</span></span>|<span data-ttu-id="d5491-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5491-111">Boolean</span></span>|<span data-ttu-id="d5491-112">Se o estoque é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="d5491-112">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="d5491-113">modernApps</span><span class="sxs-lookup"><span data-stu-id="d5491-113">modernApps</span></span>|<span data-ttu-id="d5491-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5491-114">Boolean</span></span>|<span data-ttu-id="d5491-115">Se o aplicativo moderno é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="d5491-115">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="d5491-116">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="d5491-116">resourceAccess</span></span>|<span data-ttu-id="d5491-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5491-117">Boolean</span></span>|<span data-ttu-id="d5491-118">Se o acesso ao recurso é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="d5491-118">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="d5491-119">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="d5491-119">deviceConfiguration</span></span>|<span data-ttu-id="d5491-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5491-120">Boolean</span></span>|<span data-ttu-id="d5491-121">Se a configuração do dispositivo é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="d5491-121">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="d5491-122">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="d5491-122">compliancePolicy</span></span>|<span data-ttu-id="d5491-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5491-123">Boolean</span></span>|<span data-ttu-id="d5491-124">Se a política de conformidade é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="d5491-124">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="d5491-125">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="d5491-125">windowsUpdateForBusiness</span></span>|<span data-ttu-id="d5491-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="d5491-126">Boolean</span></span>|<span data-ttu-id="d5491-127">Se o Windows Update para Empresas é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="d5491-127">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5491-128">Relações</span><span class="sxs-lookup"><span data-stu-id="d5491-128">Relationships</span></span>
<span data-ttu-id="d5491-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d5491-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5491-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d5491-130">JSON Representation</span></span>
<span data-ttu-id="d5491-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d5491-131">Here is a JSON representation of the resource.</span></span>
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



