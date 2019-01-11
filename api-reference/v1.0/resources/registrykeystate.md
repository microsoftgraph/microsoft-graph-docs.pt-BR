---
title: tipo de recurso de registryKeyState
description: Contém informações sobre alterações de chave do registro relacionadas ao alerta e o processo que foi alterado as chaves do registro.
localization_priority: Normal
ms.openlocfilehash: 688c690083e24dc6c8ee7229498910befd0fdf3e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884823"
---
# <a name="registrykeystate-resource-type"></a><span data-ttu-id="7d1a6-103">tipo de recurso de registryKeyState</span><span class="sxs-lookup"><span data-stu-id="7d1a6-103">registryKeyState resource type</span></span>

<span data-ttu-id="7d1a6-104">Contém informações sobre alterações de chave do registro relacionadas ao alerta e o processo que foi alterado as chaves do registro.</span><span class="sxs-lookup"><span data-stu-id="7d1a6-104">Contains information about registry key changes related to the alert, and the process that changed the registry keys.</span></span>

## <a name="properties"></a><span data-ttu-id="7d1a6-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7d1a6-105">Properties</span></span>

| <span data-ttu-id="7d1a6-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d1a6-106">Property</span></span>     | <span data-ttu-id="7d1a6-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d1a6-107">Type</span></span>        | <span data-ttu-id="7d1a6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d1a6-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7d1a6-109">hive</span><span class="sxs-lookup"><span data-stu-id="7d1a6-109">hive</span></span>|<span data-ttu-id="7d1a6-110">registryHive</span><span class="sxs-lookup"><span data-stu-id="7d1a6-110">registryHive</span></span>|<span data-ttu-id="7d1a6-111">Uma [seção de registro do Windows](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives) :</span><span class="sxs-lookup"><span data-stu-id="7d1a6-111">A [Windows registry hive](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives) :</span></span> <ul><li><span data-ttu-id="7d1a6-112">HKEY_CURRENT_CONFIG</span><span class="sxs-lookup"><span data-stu-id="7d1a6-112">HKEY_CURRENT_CONFIG</span></span></li> <li><span data-ttu-id="7d1a6-113">HKEY_CURRENT_USER</span><span class="sxs-lookup"><span data-stu-id="7d1a6-113">HKEY_CURRENT_USER</span></span></li> <li><span data-ttu-id="7d1a6-114">HKEY_LOCAL_MACHINE\SAM</span><span class="sxs-lookup"><span data-stu-id="7d1a6-114">HKEY_LOCAL_MACHINE\SAM</span></span></li> <li><span data-ttu-id="7d1a6-115">HKEY_LOCAL_MACHINE\Security</span><span class="sxs-lookup"><span data-stu-id="7d1a6-115">HKEY_LOCAL_MACHINE\Security</span></span></li> <li><span data-ttu-id="7d1a6-116">HKEY_LOCAL_MACHINE\Software</span><span class="sxs-lookup"><span data-stu-id="7d1a6-116">HKEY_LOCAL_MACHINE\Software</span></span></li> <li><span data-ttu-id="7d1a6-117">HKEY_LOCAL_MACHINE\SYSTEM</span><span class="sxs-lookup"><span data-stu-id="7d1a6-117">HKEY_LOCAL_MACHINE\System</span></span></li> <li><span data-ttu-id="7d1a6-118">HKEY_USERS\\. Padrão.</span><span class="sxs-lookup"><span data-stu-id="7d1a6-118">HKEY_USERS\\.Default.</span></span></li></ul> <span data-ttu-id="7d1a6-119">Os valores possíveis são: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSamSoftware`, `localMachineSystem`, `usersDefault`.</span><span class="sxs-lookup"><span data-stu-id="7d1a6-119">Possible values are: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSamSoftware`, `localMachineSystem`, `usersDefault`.</span></span>|
|<span data-ttu-id="7d1a6-120">key</span><span class="sxs-lookup"><span data-stu-id="7d1a6-120">key</span></span>|<span data-ttu-id="7d1a6-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d1a6-121">String</span></span>|<span data-ttu-id="7d1a6-122">Chave de registro (ou seja alterado) atual (exclui HIVE).</span><span class="sxs-lookup"><span data-stu-id="7d1a6-122">Current (i.e. changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="7d1a6-123">oldKey</span><span class="sxs-lookup"><span data-stu-id="7d1a6-123">oldKey</span></span>|<span data-ttu-id="7d1a6-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d1a6-124">String</span></span>|<span data-ttu-id="7d1a6-125">Anterior (isto é, antes de o alterado) chave do registro (exclui HIVE).</span><span class="sxs-lookup"><span data-stu-id="7d1a6-125">Previous (i.e. before changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="7d1a6-126">oldValueData</span><span class="sxs-lookup"><span data-stu-id="7d1a6-126">oldValueData</span></span>|<span data-ttu-id="7d1a6-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d1a6-127">String</span></span>|<span data-ttu-id="7d1a6-128">Anterior (isto é, antes de o alterado) dados do valor da chave do registro (conteúdo).</span><span class="sxs-lookup"><span data-stu-id="7d1a6-128">Previous (i.e. before changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="7d1a6-129">oldValueName</span><span class="sxs-lookup"><span data-stu-id="7d1a6-129">oldValueName</span></span>|<span data-ttu-id="7d1a6-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d1a6-130">String</span></span>|<span data-ttu-id="7d1a6-131">Anterior (isto é, antes de o alterado) nome do valor da chave do registro.</span><span class="sxs-lookup"><span data-stu-id="7d1a6-131">Previous (i.e. before changed) registry key value name.</span></span>|
|<span data-ttu-id="7d1a6-132">operação</span><span class="sxs-lookup"><span data-stu-id="7d1a6-132">operation</span></span>|<span data-ttu-id="7d1a6-133">registryOperation</span><span class="sxs-lookup"><span data-stu-id="7d1a6-133">registryOperation</span></span>|<span data-ttu-id="7d1a6-134">Operação que foi alterado o nome da chave do registro e/ou valor.</span><span class="sxs-lookup"><span data-stu-id="7d1a6-134">Operation that changed the registry key name and/or value.</span></span> <span data-ttu-id="7d1a6-135">Os valores possíveis são: `unknown`, `create`, `modify`, `delete`.</span><span class="sxs-lookup"><span data-stu-id="7d1a6-135">Possible values are: `unknown`, `create`, `modify`, `delete`.</span></span>|
|<span data-ttu-id="7d1a6-136">processId</span><span class="sxs-lookup"><span data-stu-id="7d1a6-136">processId</span></span>|<span data-ttu-id="7d1a6-137">Int32</span><span class="sxs-lookup"><span data-stu-id="7d1a6-137">Int32</span></span>|<span data-ttu-id="7d1a6-138">Processo de identificação (PID) do processo que modificou a chave do registro (processo detalhes aparecerão na coleção alerta 'processos').</span><span class="sxs-lookup"><span data-stu-id="7d1a6-138">Process ID (PID) of the process that modified the registry key (process details will appear in the alert 'processes' collection).</span></span>|
|<span data-ttu-id="7d1a6-139">valueData</span><span class="sxs-lookup"><span data-stu-id="7d1a6-139">valueData</span></span>|<span data-ttu-id="7d1a6-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d1a6-140">String</span></span>|<span data-ttu-id="7d1a6-141">Dados de valor da chave do registro (ou seja alterado) atual (conteúdo).</span><span class="sxs-lookup"><span data-stu-id="7d1a6-141">Current (i.e. changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="7d1a6-142">valueName</span><span class="sxs-lookup"><span data-stu-id="7d1a6-142">valueName</span></span>|<span data-ttu-id="7d1a6-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d1a6-143">String</span></span>|<span data-ttu-id="7d1a6-144">Nome do valor da chave do registro (ou seja alterado) atual</span><span class="sxs-lookup"><span data-stu-id="7d1a6-144">Current (i.e. changed) registry key value name</span></span>|
|<span data-ttu-id="7d1a6-145">valueType</span><span class="sxs-lookup"><span data-stu-id="7d1a6-145">valueType</span></span>|<span data-ttu-id="7d1a6-146">registryValueType</span><span class="sxs-lookup"><span data-stu-id="7d1a6-146">registryValueType</span></span>|[<span data-ttu-id="7d1a6-147">Tipo de valor da chave do registro</span><span class="sxs-lookup"><span data-stu-id="7d1a6-147">Registry key value type</span></span>](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types) <ul><li><span data-ttu-id="7d1a6-148">REG_BINARY</span><span class="sxs-lookup"><span data-stu-id="7d1a6-148">REG_BINARY</span></span></li> <li><span data-ttu-id="7d1a6-149">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="7d1a6-149">REG_DWORD</span></span></li> <li><span data-ttu-id="7d1a6-150">REG_DWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="7d1a6-150">REG_DWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="7d1a6-151">REG_DWORD_BIG_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="7d1a6-151">REG_DWORD_BIG_ENDIAN</span></span></li><li><span data-ttu-id="7d1a6-152">REG_EXPAND_SZ</span><span class="sxs-lookup"><span data-stu-id="7d1a6-152">REG_EXPAND_SZ</span></span></li> <li><span data-ttu-id="7d1a6-153">REG_LINK</span><span class="sxs-lookup"><span data-stu-id="7d1a6-153">REG_LINK</span></span></li> <li><span data-ttu-id="7d1a6-154">REG_MULTI_SZ</span><span class="sxs-lookup"><span data-stu-id="7d1a6-154">REG_MULTI_SZ</span></span></li> <li><span data-ttu-id="7d1a6-155">REG_NONE</span><span class="sxs-lookup"><span data-stu-id="7d1a6-155">REG_NONE</span></span></li> <li><span data-ttu-id="7d1a6-156">REG_QWORD</span><span class="sxs-lookup"><span data-stu-id="7d1a6-156">REG_QWORD</span></span></li> <li><span data-ttu-id="7d1a6-157">REG_QWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="7d1a6-157">REG_QWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="7d1a6-158">REG_SZ</span><span class="sxs-lookup"><span data-stu-id="7d1a6-158">REG_SZ</span></span></li></ul> <span data-ttu-id="7d1a6-159">Os valores possíveis são: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.</span><span class="sxs-lookup"><span data-stu-id="7d1a6-159">Possible values are: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7d1a6-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7d1a6-160">JSON representation</span></span>

<span data-ttu-id="7d1a6-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7d1a6-161">The following is a JSON representation of the resource.</span></span>

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
