---
title: tipo de recurso securityBaselineSettingState
description: O estado de conformidade da linha de base de segurança de uma configuração para um dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ab5dd14c0929c58b9c076d1115d487e560d80333
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522577"
---
# <a name="securitybaselinesettingstate-resource-type"></a><span data-ttu-id="db003-103">tipo de recurso securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="db003-103">securityBaselineSettingState resource type</span></span>

> <span data-ttu-id="db003-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="db003-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db003-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="db003-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db003-106">O estado de conformidade da linha de base de segurança de uma configuração para um dispositivo</span><span class="sxs-lookup"><span data-stu-id="db003-106">The security baseline compliance state of a setting for a device</span></span>

## <a name="methods"></a><span data-ttu-id="db003-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="db003-107">Methods</span></span>
|<span data-ttu-id="db003-108">Método</span><span class="sxs-lookup"><span data-stu-id="db003-108">Method</span></span>|<span data-ttu-id="db003-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="db003-109">Return Type</span></span>|<span data-ttu-id="db003-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="db003-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="db003-111">Listar securityBaselineSettingStates</span><span class="sxs-lookup"><span data-stu-id="db003-111">List securityBaselineSettingStates</span></span>](../api/intune-deviceintent-securitybaselinesettingstate-list.md)|<span data-ttu-id="db003-112">coleção [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)</span><span class="sxs-lookup"><span data-stu-id="db003-112">[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) collection</span></span>|<span data-ttu-id="db003-113">Listar Propriedades e relações dos objetos [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="db003-113">List properties and relationships of the [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) objects.</span></span>|
|[<span data-ttu-id="db003-114">Obter securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="db003-114">Get securityBaselineSettingState</span></span>](../api/intune-deviceintent-securitybaselinesettingstate-get.md)|[<span data-ttu-id="db003-115">securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="db003-115">securityBaselineSettingState</span></span>](../resources/intune-deviceintent-securitybaselinesettingstate.md)|<span data-ttu-id="db003-116">Leia as propriedades e as relações do objeto [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="db003-116">Read properties and relationships of the [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object.</span></span>|
|[<span data-ttu-id="db003-117">Criar securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="db003-117">Create securityBaselineSettingState</span></span>](../api/intune-deviceintent-securitybaselinesettingstate-create.md)|[<span data-ttu-id="db003-118">securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="db003-118">securityBaselineSettingState</span></span>](../resources/intune-deviceintent-securitybaselinesettingstate.md)|<span data-ttu-id="db003-119">Criar um novo objeto [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="db003-119">Create a new [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object.</span></span>|
|[<span data-ttu-id="db003-120">Excluir securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="db003-120">Delete securityBaselineSettingState</span></span>](../api/intune-deviceintent-securitybaselinesettingstate-delete.md)|<span data-ttu-id="db003-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="db003-121">None</span></span>|<span data-ttu-id="db003-122">Exclui [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="db003-122">Deletes a [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md).</span></span>|
|[<span data-ttu-id="db003-123">Atualizar securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="db003-123">Update securityBaselineSettingState</span></span>](../api/intune-deviceintent-securitybaselinesettingstate-update.md)|[<span data-ttu-id="db003-124">securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="db003-124">securityBaselineSettingState</span></span>](../resources/intune-deviceintent-securitybaselinesettingstate.md)|<span data-ttu-id="db003-125">Atualiza as propriedades de um objeto [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="db003-125">Update the properties of a [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="db003-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="db003-126">Properties</span></span>
|<span data-ttu-id="db003-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db003-127">Property</span></span>|<span data-ttu-id="db003-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="db003-128">Type</span></span>|<span data-ttu-id="db003-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="db003-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db003-130">id</span><span class="sxs-lookup"><span data-stu-id="db003-130">id</span></span>|<span data-ttu-id="db003-131">String</span><span class="sxs-lookup"><span data-stu-id="db003-131">String</span></span>|<span data-ttu-id="db003-132">Identificador exclusivo da entidade</span><span class="sxs-lookup"><span data-stu-id="db003-132">Unique identifier of the entity</span></span>|
|<span data-ttu-id="db003-133">settingName</span><span class="sxs-lookup"><span data-stu-id="db003-133">settingName</span></span>|<span data-ttu-id="db003-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db003-134">String</span></span>|<span data-ttu-id="db003-135">O nome da configuração que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="db003-135">The setting name that is being reported</span></span>|
|<span data-ttu-id="db003-136">state</span><span class="sxs-lookup"><span data-stu-id="db003-136">state</span></span>|[<span data-ttu-id="db003-137">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="db003-137">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="db003-138">O estado de conformidade da configuração da linha de base de segurança.</span><span class="sxs-lookup"><span data-stu-id="db003-138">The compliance state of the security baseline setting.</span></span> <span data-ttu-id="db003-139">Os valores possíveis são: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="db003-139">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="db003-140">settingCategoryId</span><span class="sxs-lookup"><span data-stu-id="db003-140">settingCategoryId</span></span>|<span data-ttu-id="db003-141">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="db003-141">String</span></span>|<span data-ttu-id="db003-142">A ID da categoria de configuração à qual essa configuração pertence</span><span class="sxs-lookup"><span data-stu-id="db003-142">The setting category id which this setting belongs to</span></span>|

## <a name="relationships"></a><span data-ttu-id="db003-143">Relações</span><span class="sxs-lookup"><span data-stu-id="db003-143">Relationships</span></span>
<span data-ttu-id="db003-144">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="db003-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="db003-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="db003-145">JSON Representation</span></span>
<span data-ttu-id="db003-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="db003-146">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineSettingState",
  "id": "String (identifier)",
  "settingName": "String",
  "state": "String",
  "settingCategoryId": "String"
}
```



