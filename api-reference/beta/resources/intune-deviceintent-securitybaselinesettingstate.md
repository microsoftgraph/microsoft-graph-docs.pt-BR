---
title: tipo de recurso securityBaselineSettingState
description: O estado de conformidade da linha de base de segurança de uma configuração para um dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ab5dd14c0929c58b9c076d1115d487e560d80333
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562276"
---
# <a name="securitybaselinesettingstate-resource-type"></a><span data-ttu-id="3b95a-103">tipo de recurso securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="3b95a-103">securityBaselineSettingState resource type</span></span>

> <span data-ttu-id="3b95a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3b95a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b95a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3b95a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b95a-106">O estado de conformidade da linha de base de segurança de uma configuração para um dispositivo</span><span class="sxs-lookup"><span data-stu-id="3b95a-106">The security baseline compliance state of a setting for a device</span></span>

## <a name="methods"></a><span data-ttu-id="3b95a-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="3b95a-107">Methods</span></span>
|<span data-ttu-id="3b95a-108">Método</span><span class="sxs-lookup"><span data-stu-id="3b95a-108">Method</span></span>|<span data-ttu-id="3b95a-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3b95a-109">Return Type</span></span>|<span data-ttu-id="3b95a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b95a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3b95a-111">Listar securityBaselineSettingStates</span><span class="sxs-lookup"><span data-stu-id="3b95a-111">List securityBaselineSettingStates</span></span>](../api/intune-deviceintent-securitybaselinesettingstate-list.md)|<span data-ttu-id="3b95a-112">coleção [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)</span><span class="sxs-lookup"><span data-stu-id="3b95a-112">[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) collection</span></span>|<span data-ttu-id="3b95a-113">Listar Propriedades e relações dos objetos [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="3b95a-113">List properties and relationships of the [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) objects.</span></span>|
|[<span data-ttu-id="3b95a-114">Obter securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="3b95a-114">Get securityBaselineSettingState</span></span>](../api/intune-deviceintent-securitybaselinesettingstate-get.md)|[<span data-ttu-id="3b95a-115">securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="3b95a-115">securityBaselineSettingState</span></span>](../resources/intune-deviceintent-securitybaselinesettingstate.md)|<span data-ttu-id="3b95a-116">Leia as propriedades e as relações do objeto [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="3b95a-116">Read properties and relationships of the [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object.</span></span>|
|[<span data-ttu-id="3b95a-117">Criar securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="3b95a-117">Create securityBaselineSettingState</span></span>](../api/intune-deviceintent-securitybaselinesettingstate-create.md)|[<span data-ttu-id="3b95a-118">securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="3b95a-118">securityBaselineSettingState</span></span>](../resources/intune-deviceintent-securitybaselinesettingstate.md)|<span data-ttu-id="3b95a-119">Criar um novo objeto [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="3b95a-119">Create a new [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object.</span></span>|
|[<span data-ttu-id="3b95a-120">Excluir securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="3b95a-120">Delete securityBaselineSettingState</span></span>](../api/intune-deviceintent-securitybaselinesettingstate-delete.md)|<span data-ttu-id="3b95a-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3b95a-121">None</span></span>|<span data-ttu-id="3b95a-122">Exclui [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="3b95a-122">Deletes a [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md).</span></span>|
|[<span data-ttu-id="3b95a-123">Atualizar securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="3b95a-123">Update securityBaselineSettingState</span></span>](../api/intune-deviceintent-securitybaselinesettingstate-update.md)|[<span data-ttu-id="3b95a-124">securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="3b95a-124">securityBaselineSettingState</span></span>](../resources/intune-deviceintent-securitybaselinesettingstate.md)|<span data-ttu-id="3b95a-125">Atualiza as propriedades de um objeto [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="3b95a-125">Update the properties of a [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3b95a-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3b95a-126">Properties</span></span>
|<span data-ttu-id="3b95a-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b95a-127">Property</span></span>|<span data-ttu-id="3b95a-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b95a-128">Type</span></span>|<span data-ttu-id="3b95a-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b95a-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b95a-130">id</span><span class="sxs-lookup"><span data-stu-id="3b95a-130">id</span></span>|<span data-ttu-id="3b95a-131">String</span><span class="sxs-lookup"><span data-stu-id="3b95a-131">String</span></span>|<span data-ttu-id="3b95a-132">Identificador exclusivo da entidade</span><span class="sxs-lookup"><span data-stu-id="3b95a-132">Unique identifier of the entity</span></span>|
|<span data-ttu-id="3b95a-133">settingName</span><span class="sxs-lookup"><span data-stu-id="3b95a-133">settingName</span></span>|<span data-ttu-id="3b95a-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b95a-134">String</span></span>|<span data-ttu-id="3b95a-135">O nome da configuração que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="3b95a-135">The setting name that is being reported</span></span>|
|<span data-ttu-id="3b95a-136">estado</span><span class="sxs-lookup"><span data-stu-id="3b95a-136">state</span></span>|[<span data-ttu-id="3b95a-137">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="3b95a-137">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="3b95a-138">O estado de conformidade da configuração da linha de base de segurança.</span><span class="sxs-lookup"><span data-stu-id="3b95a-138">The compliance state of the security baseline setting.</span></span> <span data-ttu-id="3b95a-139">Os possíveis valores são: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="3b95a-139">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="3b95a-140">settingCategoryId</span><span class="sxs-lookup"><span data-stu-id="3b95a-140">settingCategoryId</span></span>|<span data-ttu-id="3b95a-141">String</span><span class="sxs-lookup"><span data-stu-id="3b95a-141">String</span></span>|<span data-ttu-id="3b95a-142">A ID da categoria de configuração à qual essa configuração pertence</span><span class="sxs-lookup"><span data-stu-id="3b95a-142">The setting category id which this setting belongs to</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b95a-143">Relações</span><span class="sxs-lookup"><span data-stu-id="3b95a-143">Relationships</span></span>
<span data-ttu-id="3b95a-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3b95a-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3b95a-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3b95a-145">JSON Representation</span></span>
<span data-ttu-id="3b95a-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3b95a-146">Here is a JSON representation of the resource.</span></span>
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



