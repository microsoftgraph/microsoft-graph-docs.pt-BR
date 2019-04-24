---
title: Tipo de recurso configurationManagerClientEnabledFeatures
description: recursos habilitados pelo cliente do Gerenciador de Configurações
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 91ffd0180660b33e9ead5210f9b23870af18e29a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32467306"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="d5fb2-103">Tipo de recurso configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="d5fb2-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="d5fb2-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d5fb2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5fb2-105">recursos habilitados pelo cliente do Gerenciador de Configurações</span><span class="sxs-lookup"><span data-stu-id="d5fb2-105">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="d5fb2-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d5fb2-106">Properties</span></span>
|<span data-ttu-id="d5fb2-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5fb2-107">Property</span></span>|<span data-ttu-id="d5fb2-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5fb2-108">Type</span></span>|<span data-ttu-id="d5fb2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5fb2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5fb2-110">inventory</span><span class="sxs-lookup"><span data-stu-id="d5fb2-110">inventory</span></span>|<span data-ttu-id="d5fb2-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="d5fb2-111">Boolean</span></span>|<span data-ttu-id="d5fb2-112">Se o estoque é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="d5fb2-112">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="d5fb2-113">modernApps</span><span class="sxs-lookup"><span data-stu-id="d5fb2-113">modernApps</span></span>|<span data-ttu-id="d5fb2-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="d5fb2-114">Boolean</span></span>|<span data-ttu-id="d5fb2-115">Se o aplicativo moderno é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="d5fb2-115">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="d5fb2-116">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="d5fb2-116">resourceAccess</span></span>|<span data-ttu-id="d5fb2-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="d5fb2-117">Boolean</span></span>|<span data-ttu-id="d5fb2-118">Se o acesso ao recurso é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="d5fb2-118">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="d5fb2-119">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="d5fb2-119">deviceConfiguration</span></span>|<span data-ttu-id="d5fb2-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="d5fb2-120">Boolean</span></span>|<span data-ttu-id="d5fb2-121">Se a configuração do dispositivo é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="d5fb2-121">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="d5fb2-122">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="d5fb2-122">compliancePolicy</span></span>|<span data-ttu-id="d5fb2-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="d5fb2-123">Boolean</span></span>|<span data-ttu-id="d5fb2-124">Se a política de conformidade é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="d5fb2-124">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="d5fb2-125">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="d5fb2-125">windowsUpdateForBusiness</span></span>|<span data-ttu-id="d5fb2-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="d5fb2-126">Boolean</span></span>|<span data-ttu-id="d5fb2-127">Se o Windows Update para Empresas é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="d5fb2-127">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5fb2-128">Relações</span><span class="sxs-lookup"><span data-stu-id="d5fb2-128">Relationships</span></span>
<span data-ttu-id="d5fb2-129">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d5fb2-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5fb2-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d5fb2-130">JSON Representation</span></span>
<span data-ttu-id="d5fb2-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d5fb2-131">Here is a JSON representation of the resource.</span></span>
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



