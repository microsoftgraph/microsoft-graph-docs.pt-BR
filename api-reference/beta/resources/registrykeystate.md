---
title: tipo de recurso registryKeystate
description: Contém informações sobre as alterações da chave do registro relacionadas ao alerta e o processo que alterou as chaves do registro.
localization_priority: Normal
ms.openlocfilehash: d07b0b6f502794154b400444eaf3854535e04547
ms.sourcegitcommit: a4773239d8559899c3f9433b3073e250a56d2e04
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/13/2019
ms.locfileid: "29994423"
---
# <a name="registrykeystate-resource-type"></a><span data-ttu-id="bc0b0-103">tipo de recurso registryKeystate</span><span class="sxs-lookup"><span data-stu-id="bc0b0-103">registryKeyState resource type</span></span>

<span data-ttu-id="bc0b0-104">Contém informações sobre as alterações da chave do registro relacionadas ao alerta e o processo que alterou as chaves do registro.</span><span class="sxs-lookup"><span data-stu-id="bc0b0-104">Contains information about registry key changes related to the alert, and the process that changed the registry keys.</span></span>

## <a name="properties"></a><span data-ttu-id="bc0b0-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bc0b0-105">Properties</span></span>

| <span data-ttu-id="bc0b0-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc0b0-106">Property</span></span>     | <span data-ttu-id="bc0b0-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc0b0-107">Type</span></span>        | <span data-ttu-id="bc0b0-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc0b0-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bc0b0-109">Hive</span><span class="sxs-lookup"><span data-stu-id="bc0b0-109">hive</span></span>|<span data-ttu-id="bc0b0-110">registryHive</span><span class="sxs-lookup"><span data-stu-id="bc0b0-110">registryHive</span></span>|<span data-ttu-id="bc0b0-111">Uma [seção de registro do Windows](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives) :</span><span class="sxs-lookup"><span data-stu-id="bc0b0-111">A [Windows registry hive](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives) :</span></span> <ul><li><span data-ttu-id="bc0b0-112">HKEY_CURRENT_CONFIG</span><span class="sxs-lookup"><span data-stu-id="bc0b0-112">HKEY_CURRENT_CONFIG</span></span></li> <li><span data-ttu-id="bc0b0-113">HKEY_CURRENT_USER</span><span class="sxs-lookup"><span data-stu-id="bc0b0-113">HKEY_CURRENT_USER</span></span></li> <li><span data-ttu-id="bc0b0-114">HKEY_LOCAL_MACHINE\SAM</span><span class="sxs-lookup"><span data-stu-id="bc0b0-114">HKEY_LOCAL_MACHINE\SAM</span></span></li> <li><span data-ttu-id="bc0b0-115">HKEY_LOCAL_MACHINE\Security</span><span class="sxs-lookup"><span data-stu-id="bc0b0-115">HKEY_LOCAL_MACHINE\Security</span></span></li> <li><span data-ttu-id="bc0b0-116">HKEY_LOCAL_MACHINE\Software</span><span class="sxs-lookup"><span data-stu-id="bc0b0-116">HKEY_LOCAL_MACHINE\Software</span></span></li> <li><span data-ttu-id="bc0b0-117">HKEY_LOCAL_MACHINE\System</span><span class="sxs-lookup"><span data-stu-id="bc0b0-117">HKEY_LOCAL_MACHINE\System</span></span></li> <li><span data-ttu-id="bc0b0-118">HKEY_USERS\\. Será.</span><span class="sxs-lookup"><span data-stu-id="bc0b0-118">HKEY_USERS\\.Default.</span></span></li></ul> <span data-ttu-id="bc0b0-119">Os valores possíveis são: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSecurity`, `localMachineSoftware`, `localMachineSystem`, `usersDefault`.</span><span class="sxs-lookup"><span data-stu-id="bc0b0-119">Possible values are: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSecurity`, `localMachineSoftware`, `localMachineSystem`, `usersDefault`.</span></span>|
|<span data-ttu-id="bc0b0-120">chave</span><span class="sxs-lookup"><span data-stu-id="bc0b0-120">key</span></span>|<span data-ttu-id="bc0b0-121">String</span><span class="sxs-lookup"><span data-stu-id="bc0b0-121">String</span></span>|<span data-ttu-id="bc0b0-122">Chave de registro atual (ou seja, alterada) (exclui HIVE).</span><span class="sxs-lookup"><span data-stu-id="bc0b0-122">Current (i.e. changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="bc0b0-123">oldKey</span><span class="sxs-lookup"><span data-stu-id="bc0b0-123">oldKey</span></span>|<span data-ttu-id="bc0b0-124">String</span><span class="sxs-lookup"><span data-stu-id="bc0b0-124">String</span></span>|<span data-ttu-id="bc0b0-125">Chave de registro anterior (ou seja, antes da alteração) (exclui HIVE).</span><span class="sxs-lookup"><span data-stu-id="bc0b0-125">Previous (i.e. before changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="bc0b0-126">oldValueData</span><span class="sxs-lookup"><span data-stu-id="bc0b0-126">oldValueData</span></span>|<span data-ttu-id="bc0b0-127">String</span><span class="sxs-lookup"><span data-stu-id="bc0b0-127">String</span></span>|<span data-ttu-id="bc0b0-128">Dados anteriores (ou seja, antes da alteração) dos valores da chave do registro (conteúdo).</span><span class="sxs-lookup"><span data-stu-id="bc0b0-128">Previous (i.e. before changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="bc0b0-129">oldValue</span><span class="sxs-lookup"><span data-stu-id="bc0b0-129">oldValueName</span></span>|<span data-ttu-id="bc0b0-130">String</span><span class="sxs-lookup"><span data-stu-id="bc0b0-130">String</span></span>|<span data-ttu-id="bc0b0-131">Nome do valor da chave anterior (ou seja, antes da alteração).</span><span class="sxs-lookup"><span data-stu-id="bc0b0-131">Previous (i.e. before changed) registry key value name.</span></span>|
|<span data-ttu-id="bc0b0-132">operações</span><span class="sxs-lookup"><span data-stu-id="bc0b0-132">operation</span></span>|<span data-ttu-id="bc0b0-133">registryOperation</span><span class="sxs-lookup"><span data-stu-id="bc0b0-133">registryOperation</span></span>|<span data-ttu-id="bc0b0-134">Operação que alterou o nome da chave do registro e/ou o valor.</span><span class="sxs-lookup"><span data-stu-id="bc0b0-134">Operation that changed the registry key name and/or value.</span></span> <span data-ttu-id="bc0b0-135">Os valores possíveis são: `unknown`, `create`, `modify`, `delete`.</span><span class="sxs-lookup"><span data-stu-id="bc0b0-135">Possible values are: `unknown`, `create`, `modify`, `delete`.</span></span>|
|<span data-ttu-id="bc0b0-136">Identificação</span><span class="sxs-lookup"><span data-stu-id="bc0b0-136">processId</span></span>|<span data-ttu-id="bc0b0-137">Int32</span><span class="sxs-lookup"><span data-stu-id="bc0b0-137">Int32</span></span>|<span data-ttu-id="bc0b0-138">ID de processo (PID) do processo que modificou a chave de registro (os detalhes do processo aparecerão na coleção Alert ' Processes ').</span><span class="sxs-lookup"><span data-stu-id="bc0b0-138">Process ID (PID) of the process that modified the registry key (process details will appear in the alert 'processes' collection).</span></span>|
|<span data-ttu-id="bc0b0-139">valueData</span><span class="sxs-lookup"><span data-stu-id="bc0b0-139">valueData</span></span>|<span data-ttu-id="bc0b0-140">String</span><span class="sxs-lookup"><span data-stu-id="bc0b0-140">String</span></span>|<span data-ttu-id="bc0b0-141">Dados de valores de chave de registro (conteúdo) atuais (ou seja, alterados).</span><span class="sxs-lookup"><span data-stu-id="bc0b0-141">Current (i.e. changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="bc0b0-142">valueName</span><span class="sxs-lookup"><span data-stu-id="bc0b0-142">valueName</span></span>|<span data-ttu-id="bc0b0-143">String</span><span class="sxs-lookup"><span data-stu-id="bc0b0-143">String</span></span>|<span data-ttu-id="bc0b0-144">Nome do valor da chave do registro atual (ou seja, alterado)</span><span class="sxs-lookup"><span data-stu-id="bc0b0-144">Current (i.e. changed) registry key value name</span></span>|
|<span data-ttu-id="bc0b0-145">valueType</span><span class="sxs-lookup"><span data-stu-id="bc0b0-145">valueType</span></span>|<span data-ttu-id="bc0b0-146">registryValueType</span><span class="sxs-lookup"><span data-stu-id="bc0b0-146">registryValueType</span></span>|[<span data-ttu-id="bc0b0-147">Tipo de valor da chave do registro</span><span class="sxs-lookup"><span data-stu-id="bc0b0-147">Registry key value type</span></span>](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types) <ul><li><span data-ttu-id="bc0b0-148">REG_BINARY</span><span class="sxs-lookup"><span data-stu-id="bc0b0-148">REG_BINARY</span></span></li> <li><span data-ttu-id="bc0b0-149">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="bc0b0-149">REG_DWORD</span></span></li> <li><span data-ttu-id="bc0b0-150">REG_DWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="bc0b0-150">REG_DWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="bc0b0-151">REG_DWORD_BIG_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="bc0b0-151">REG_DWORD_BIG_ENDIAN</span></span></li><li><span data-ttu-id="bc0b0-152">REG_EXPAND_SZ</span><span class="sxs-lookup"><span data-stu-id="bc0b0-152">REG_EXPAND_SZ</span></span></li> <li><span data-ttu-id="bc0b0-153">REG_LINK</span><span class="sxs-lookup"><span data-stu-id="bc0b0-153">REG_LINK</span></span></li> <li><span data-ttu-id="bc0b0-154">REG_MULTI_SZ</span><span class="sxs-lookup"><span data-stu-id="bc0b0-154">REG_MULTI_SZ</span></span></li> <li><span data-ttu-id="bc0b0-155">REG_NONE</span><span class="sxs-lookup"><span data-stu-id="bc0b0-155">REG_NONE</span></span></li> <li><span data-ttu-id="bc0b0-156">REG_QWORD</span><span class="sxs-lookup"><span data-stu-id="bc0b0-156">REG_QWORD</span></span></li> <li><span data-ttu-id="bc0b0-157">REG_QWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="bc0b0-157">REG_QWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="bc0b0-158">REG_SZ</span><span class="sxs-lookup"><span data-stu-id="bc0b0-158">REG_SZ</span></span></li></ul> <span data-ttu-id="bc0b0-159">Os valores possíveis são: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.</span><span class="sxs-lookup"><span data-stu-id="bc0b0-159">Possible values are: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bc0b0-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bc0b0-160">JSON representation</span></span>

<span data-ttu-id="bc0b0-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bc0b0-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.registryKeyState"
}-->

```json
{
  "hive": "@odata.type: microsoft.graph.registryHive",
  "key": "String",
  "oldKey": "String",
  "oldValueData": "String",
  "oldValueName": "String",
  "operation": "@odata.type: microsoft.graph.registryOperation",
  "processId": 1024,
  "valueData": "String",
  "valueName": "String",
  "valueType": "@odata.type: microsoft.graph.registryValueType"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "registryKeyState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
