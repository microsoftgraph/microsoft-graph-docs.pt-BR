---
title: Tipo de recurso configurationManagerClientEnabledFeatures
description: recursos habilitados pelo cliente do Gerenciador de Configurações
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7975130bb047e097ea0d52a4ce770fb35e4efa32
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425901"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="d0726-103">Tipo de recurso configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="d0726-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="d0726-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="d0726-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d0726-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d0726-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d0726-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="d0726-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0726-107">recursos habilitados pelo cliente do Gerenciador de Configurações</span><span class="sxs-lookup"><span data-stu-id="d0726-107">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="d0726-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d0726-108">Properties</span></span>
|<span data-ttu-id="d0726-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d0726-109">Property</span></span>|<span data-ttu-id="d0726-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0726-110">Type</span></span>|<span data-ttu-id="d0726-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0726-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0726-112">inventory</span><span class="sxs-lookup"><span data-stu-id="d0726-112">inventory</span></span>|<span data-ttu-id="d0726-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0726-113">Boolean</span></span>|<span data-ttu-id="d0726-114">Se o estoque é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="d0726-114">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="d0726-115">modernApps</span><span class="sxs-lookup"><span data-stu-id="d0726-115">modernApps</span></span>|<span data-ttu-id="d0726-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0726-116">Boolean</span></span>|<span data-ttu-id="d0726-117">Se o aplicativo moderno é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="d0726-117">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="d0726-118">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="d0726-118">resourceAccess</span></span>|<span data-ttu-id="d0726-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0726-119">Boolean</span></span>|<span data-ttu-id="d0726-120">Se o acesso ao recurso é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="d0726-120">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="d0726-121">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="d0726-121">deviceConfiguration</span></span>|<span data-ttu-id="d0726-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0726-122">Boolean</span></span>|<span data-ttu-id="d0726-123">Se a configuração do dispositivo é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="d0726-123">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="d0726-124">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="d0726-124">compliancePolicy</span></span>|<span data-ttu-id="d0726-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0726-125">Boolean</span></span>|<span data-ttu-id="d0726-126">Se a política de conformidade é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="d0726-126">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="d0726-127">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="d0726-127">windowsUpdateForBusiness</span></span>|<span data-ttu-id="d0726-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0726-128">Boolean</span></span>|<span data-ttu-id="d0726-129">Se o Windows Update para Empresas é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="d0726-129">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0726-130">Relações</span><span class="sxs-lookup"><span data-stu-id="d0726-130">Relationships</span></span>
<span data-ttu-id="d0726-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d0726-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0726-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d0726-132">JSON Representation</span></span>
<span data-ttu-id="d0726-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d0726-133">Here is a JSON representation of the resource.</span></span>
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




