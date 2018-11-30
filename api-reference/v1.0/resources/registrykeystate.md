---
title: tipo de recurso de registryKeyState
description: Contém informações sobre alterações de chave do registro relacionadas ao alerta e o processo que foi alterado as chaves do registro.
ms.openlocfilehash: 37654aab2bf8f0afae0f7ec6ed544aed8634dacc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005316"
---
# <a name="registrykeystate-resource-type"></a><span data-ttu-id="e4f42-103">tipo de recurso de registryKeyState</span><span class="sxs-lookup"><span data-stu-id="e4f42-103">registryKeyState resource type</span></span>

<span data-ttu-id="e4f42-104">Contém informações sobre alterações de chave do registro relacionadas ao alerta e o processo que foi alterado as chaves do registro.</span><span class="sxs-lookup"><span data-stu-id="e4f42-104">Contains information about registry key changes related to the alert, and the process that changed the registry keys.</span></span>

## <a name="properties"></a><span data-ttu-id="e4f42-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e4f42-105">Properties</span></span>

| <span data-ttu-id="e4f42-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e4f42-106">Property</span></span>     | <span data-ttu-id="e4f42-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4f42-107">Type</span></span>        | <span data-ttu-id="e4f42-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4f42-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e4f42-109">hive</span><span class="sxs-lookup"><span data-stu-id="e4f42-109">hive</span></span>|<span data-ttu-id="e4f42-110">registryHive</span><span class="sxs-lookup"><span data-stu-id="e4f42-110">registryHive</span></span>|<span data-ttu-id="e4f42-111">Uma [seção de registro do Windows](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives) :</span><span class="sxs-lookup"><span data-stu-id="e4f42-111">A [Windows registry hive](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives) :</span></span> <ul><li><span data-ttu-id="e4f42-112">HKEY_CURRENT_CONFIG</span><span class="sxs-lookup"><span data-stu-id="e4f42-112">HKEY_CURRENT_CONFIG</span></span></li> <li><span data-ttu-id="e4f42-113">HKEY_CURRENT_USER</span><span class="sxs-lookup"><span data-stu-id="e4f42-113">HKEY_CURRENT_USER</span></span></li> <li><span data-ttu-id="e4f42-114">HKEY_LOCAL_MACHINE\SAM</span><span class="sxs-lookup"><span data-stu-id="e4f42-114">HKEY_LOCAL_MACHINE\SAM</span></span></li> <li><span data-ttu-id="e4f42-115">HKEY_LOCAL_MACHINE\Security</span><span class="sxs-lookup"><span data-stu-id="e4f42-115">HKEY_LOCAL_MACHINE\Security</span></span></li> <li><span data-ttu-id="e4f42-116">HKEY_LOCAL_MACHINE\Software</span><span class="sxs-lookup"><span data-stu-id="e4f42-116">HKEY_LOCAL_MACHINE\Software</span></span></li> <li><span data-ttu-id="e4f42-117">HKEY_LOCAL_MACHINE\SYSTEM</span><span class="sxs-lookup"><span data-stu-id="e4f42-117">HKEY_LOCAL_MACHINE\System</span></span></li> <li><span data-ttu-id="e4f42-118">HKEY_USERS\\. Padrão.</span><span class="sxs-lookup"><span data-stu-id="e4f42-118">HKEY_USERS\\.Default.</span></span></li></ul> <span data-ttu-id="e4f42-119">Os valores possíveis são: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSamSoftware`, `localMachineSystem`, `usersDefault`.</span><span class="sxs-lookup"><span data-stu-id="e4f42-119">Possible values are: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSamSoftware`, `localMachineSystem`, `usersDefault`.</span></span>|
|<span data-ttu-id="e4f42-120">key</span><span class="sxs-lookup"><span data-stu-id="e4f42-120">key</span></span>|<span data-ttu-id="e4f42-121">String</span><span class="sxs-lookup"><span data-stu-id="e4f42-121">String</span></span>|<span data-ttu-id="e4f42-122">Chave de registro (ou seja alterado) atual (exclui HIVE).</span><span class="sxs-lookup"><span data-stu-id="e4f42-122">Current (i.e. changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="e4f42-123">oldKey</span><span class="sxs-lookup"><span data-stu-id="e4f42-123">oldKey</span></span>|<span data-ttu-id="e4f42-124">String</span><span class="sxs-lookup"><span data-stu-id="e4f42-124">String</span></span>|<span data-ttu-id="e4f42-125">Anterior (isto é, antes de o alterado) chave do registro (exclui HIVE).</span><span class="sxs-lookup"><span data-stu-id="e4f42-125">Previous (i.e. before changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="e4f42-126">oldValueData</span><span class="sxs-lookup"><span data-stu-id="e4f42-126">oldValueData</span></span>|<span data-ttu-id="e4f42-127">String</span><span class="sxs-lookup"><span data-stu-id="e4f42-127">String</span></span>|<span data-ttu-id="e4f42-128">Anterior (isto é, antes de o alterado) dados do valor da chave do registro (conteúdo).</span><span class="sxs-lookup"><span data-stu-id="e4f42-128">Previous (i.e. before changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="e4f42-129">oldValueName</span><span class="sxs-lookup"><span data-stu-id="e4f42-129">oldValueName</span></span>|<span data-ttu-id="e4f42-130">String</span><span class="sxs-lookup"><span data-stu-id="e4f42-130">String</span></span>|<span data-ttu-id="e4f42-131">Anterior (isto é, antes de o alterado) nome do valor da chave do registro.</span><span class="sxs-lookup"><span data-stu-id="e4f42-131">Previous (i.e. before changed) registry key value name.</span></span>|
|<span data-ttu-id="e4f42-132">operação</span><span class="sxs-lookup"><span data-stu-id="e4f42-132">operation</span></span>|<span data-ttu-id="e4f42-133">registryOperation</span><span class="sxs-lookup"><span data-stu-id="e4f42-133">registryOperation</span></span>|<span data-ttu-id="e4f42-134">Operação que foi alterado o nome da chave do registro e/ou valor.</span><span class="sxs-lookup"><span data-stu-id="e4f42-134">Operation that changed the registry key name and/or value.</span></span> <span data-ttu-id="e4f42-135">Os valores possíveis são: `unknown`, `create`, `modify`, `delete`.</span><span class="sxs-lookup"><span data-stu-id="e4f42-135">Possible values are: `unknown`, `create`, `modify`, `delete`.</span></span>|
|<span data-ttu-id="e4f42-136">processId</span><span class="sxs-lookup"><span data-stu-id="e4f42-136">processId</span></span>|<span data-ttu-id="e4f42-137">Int32</span><span class="sxs-lookup"><span data-stu-id="e4f42-137">Int32</span></span>|<span data-ttu-id="e4f42-138">Processo de identificação (PID) do processo que modificou a chave do registro (processo detalhes aparecerão na coleção alerta 'processos').</span><span class="sxs-lookup"><span data-stu-id="e4f42-138">Process ID (PID) of the process that modified the registry key (process details will appear in the alert 'processes' collection).</span></span>|
|<span data-ttu-id="e4f42-139">valueData</span><span class="sxs-lookup"><span data-stu-id="e4f42-139">valueData</span></span>|<span data-ttu-id="e4f42-140">String</span><span class="sxs-lookup"><span data-stu-id="e4f42-140">String</span></span>|<span data-ttu-id="e4f42-141">Dados de valor da chave do registro (ou seja alterado) atual (conteúdo).</span><span class="sxs-lookup"><span data-stu-id="e4f42-141">Current (i.e. changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="e4f42-142">valueName</span><span class="sxs-lookup"><span data-stu-id="e4f42-142">valueName</span></span>|<span data-ttu-id="e4f42-143">String</span><span class="sxs-lookup"><span data-stu-id="e4f42-143">String</span></span>|<span data-ttu-id="e4f42-144">Nome do valor da chave do registro (ou seja alterado) atual</span><span class="sxs-lookup"><span data-stu-id="e4f42-144">Current (i.e. changed) registry key value name</span></span>|
|<span data-ttu-id="e4f42-145">valueType</span><span class="sxs-lookup"><span data-stu-id="e4f42-145">valueType</span></span>|<span data-ttu-id="e4f42-146">registryValueType</span><span class="sxs-lookup"><span data-stu-id="e4f42-146">registryValueType</span></span>|[<span data-ttu-id="e4f42-147">Tipo de valor da chave do registro</span><span class="sxs-lookup"><span data-stu-id="e4f42-147">Registry key value type</span></span>](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types) <ul><li><span data-ttu-id="e4f42-148">REG_BINARY</span><span class="sxs-lookup"><span data-stu-id="e4f42-148">REG_BINARY</span></span></li> <li><span data-ttu-id="e4f42-149">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="e4f42-149">REG_DWORD</span></span></li> <li><span data-ttu-id="e4f42-150">REG_DWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="e4f42-150">REG_DWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="e4f42-151">REG_DWORD_BIG_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="e4f42-151">REG_DWORD_BIG_ENDIAN</span></span></li><li><span data-ttu-id="e4f42-152">REG_EXPAND_SZ</span><span class="sxs-lookup"><span data-stu-id="e4f42-152">REG_EXPAND_SZ</span></span></li> <li><span data-ttu-id="e4f42-153">REG_LINK</span><span class="sxs-lookup"><span data-stu-id="e4f42-153">REG_LINK</span></span></li> <li><span data-ttu-id="e4f42-154">REG_MULTI_SZ</span><span class="sxs-lookup"><span data-stu-id="e4f42-154">REG_MULTI_SZ</span></span></li> <li><span data-ttu-id="e4f42-155">REG_NONE</span><span class="sxs-lookup"><span data-stu-id="e4f42-155">REG_NONE</span></span></li> <li><span data-ttu-id="e4f42-156">REG_QWORD</span><span class="sxs-lookup"><span data-stu-id="e4f42-156">REG_QWORD</span></span></li> <li><span data-ttu-id="e4f42-157">REG_QWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="e4f42-157">REG_QWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="e4f42-158">REG_SZ</span><span class="sxs-lookup"><span data-stu-id="e4f42-158">REG_SZ</span></span></li></ul> <span data-ttu-id="e4f42-159">Os valores possíveis são: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.</span><span class="sxs-lookup"><span data-stu-id="e4f42-159">Possible values are: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e4f42-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e4f42-160">JSON representation</span></span>

<span data-ttu-id="e4f42-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e4f42-161">The following is a JSON representation of the resource.</span></span>

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