---
title: tipo de recurso registryKeystate
description: Contém informações sobre as alterações da chave do registro relacionadas ao alerta e o processo que alterou as chaves do registro.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 10d372f2184ccbee628b59866f84678ec6c843bd
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810444"
---
# <a name="registrykeystate-resource-type"></a><span data-ttu-id="7b8bb-103">tipo de recurso registryKeystate</span><span class="sxs-lookup"><span data-stu-id="7b8bb-103">registryKeyState resource type</span></span>

<span data-ttu-id="7b8bb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b8bb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7b8bb-105">Contém informações sobre as alterações da chave do registro relacionadas ao alerta e o processo que alterou as chaves do registro.</span><span class="sxs-lookup"><span data-stu-id="7b8bb-105">Contains information about registry key changes related to the alert, and the process that changed the registry keys.</span></span>

## <a name="properties"></a><span data-ttu-id="7b8bb-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7b8bb-106">Properties</span></span>

| <span data-ttu-id="7b8bb-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b8bb-107">Property</span></span>     | <span data-ttu-id="7b8bb-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b8bb-108">Type</span></span>        | <span data-ttu-id="7b8bb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b8bb-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7b8bb-110">Hive</span><span class="sxs-lookup"><span data-stu-id="7b8bb-110">hive</span></span>|<span data-ttu-id="7b8bb-111">registryHive</span><span class="sxs-lookup"><span data-stu-id="7b8bb-111">registryHive</span></span>|<span data-ttu-id="7b8bb-112">Uma [seção de registro do Windows](/windows/desktop/sysinfo/registry-hives) :</span><span class="sxs-lookup"><span data-stu-id="7b8bb-112">A [Windows registry hive](/windows/desktop/sysinfo/registry-hives) :</span></span> <ul><li><span data-ttu-id="7b8bb-113">HKEY_CURRENT_CONFIG</span><span class="sxs-lookup"><span data-stu-id="7b8bb-113">HKEY_CURRENT_CONFIG</span></span></li> <li><span data-ttu-id="7b8bb-114">HKEY_CURRENT_USER</span><span class="sxs-lookup"><span data-stu-id="7b8bb-114">HKEY_CURRENT_USER</span></span></li> <li><span data-ttu-id="7b8bb-115">HKEY_LOCAL_MACHINE \SAM</span><span class="sxs-lookup"><span data-stu-id="7b8bb-115">HKEY_LOCAL_MACHINE\SAM</span></span></li> <li><span data-ttu-id="7b8bb-116">HKEY_LOCAL_MACHINE \Security</span><span class="sxs-lookup"><span data-stu-id="7b8bb-116">HKEY_LOCAL_MACHINE\Security</span></span></li> <li><span data-ttu-id="7b8bb-117">HKEY_LOCAL_MACHINE \Software</span><span class="sxs-lookup"><span data-stu-id="7b8bb-117">HKEY_LOCAL_MACHINE\Software</span></span></li> <li><span data-ttu-id="7b8bb-118">HKEY_LOCAL_MACHINE \System</span><span class="sxs-lookup"><span data-stu-id="7b8bb-118">HKEY_LOCAL_MACHINE\System</span></span></li> <li><span data-ttu-id="7b8bb-119">HKEY_USERS \\ . Será.</span><span class="sxs-lookup"><span data-stu-id="7b8bb-119">HKEY_USERS\\.Default.</span></span></li></ul> <span data-ttu-id="7b8bb-120">Os valores possíveis são: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSecurity`, `localMachineSoftware`, `localMachineSystem`, `usersDefault`.</span><span class="sxs-lookup"><span data-stu-id="7b8bb-120">Possible values are: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSecurity`, `localMachineSoftware`, `localMachineSystem`, `usersDefault`.</span></span>|
|<span data-ttu-id="7b8bb-121">chave</span><span class="sxs-lookup"><span data-stu-id="7b8bb-121">key</span></span>|<span data-ttu-id="7b8bb-122">String</span><span class="sxs-lookup"><span data-stu-id="7b8bb-122">String</span></span>|<span data-ttu-id="7b8bb-123">Chave de registro atual (ou seja, alterada) (exclui HIVE).</span><span class="sxs-lookup"><span data-stu-id="7b8bb-123">Current (i.e. changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="7b8bb-124">oldKey</span><span class="sxs-lookup"><span data-stu-id="7b8bb-124">oldKey</span></span>|<span data-ttu-id="7b8bb-125">String</span><span class="sxs-lookup"><span data-stu-id="7b8bb-125">String</span></span>|<span data-ttu-id="7b8bb-126">Chave de registro anterior (ou seja, antes da alteração) (exclui HIVE).</span><span class="sxs-lookup"><span data-stu-id="7b8bb-126">Previous (i.e. before changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="7b8bb-127">oldValueData</span><span class="sxs-lookup"><span data-stu-id="7b8bb-127">oldValueData</span></span>|<span data-ttu-id="7b8bb-128">String</span><span class="sxs-lookup"><span data-stu-id="7b8bb-128">String</span></span>|<span data-ttu-id="7b8bb-129">Dados anteriores (ou seja, antes da alteração) dos valores da chave do registro (conteúdo).</span><span class="sxs-lookup"><span data-stu-id="7b8bb-129">Previous (i.e. before changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="7b8bb-130">oldValue</span><span class="sxs-lookup"><span data-stu-id="7b8bb-130">oldValueName</span></span>|<span data-ttu-id="7b8bb-131">String</span><span class="sxs-lookup"><span data-stu-id="7b8bb-131">String</span></span>|<span data-ttu-id="7b8bb-132">Nome do valor da chave anterior (ou seja, antes da alteração).</span><span class="sxs-lookup"><span data-stu-id="7b8bb-132">Previous (i.e. before changed) registry key value name.</span></span>|
|<span data-ttu-id="7b8bb-133">operações</span><span class="sxs-lookup"><span data-stu-id="7b8bb-133">operation</span></span>|<span data-ttu-id="7b8bb-134">registryOperation</span><span class="sxs-lookup"><span data-stu-id="7b8bb-134">registryOperation</span></span>|<span data-ttu-id="7b8bb-135">Operação que alterou o nome da chave do registro e/ou o valor.</span><span class="sxs-lookup"><span data-stu-id="7b8bb-135">Operation that changed the registry key name and/or value.</span></span> <span data-ttu-id="7b8bb-136">Os valores possíveis são: `unknown`, `create`, `modify`, `delete`.</span><span class="sxs-lookup"><span data-stu-id="7b8bb-136">Possible values are: `unknown`, `create`, `modify`, `delete`.</span></span>|
|<span data-ttu-id="7b8bb-137">Identificação</span><span class="sxs-lookup"><span data-stu-id="7b8bb-137">processId</span></span>|<span data-ttu-id="7b8bb-138">Int32</span><span class="sxs-lookup"><span data-stu-id="7b8bb-138">Int32</span></span>|<span data-ttu-id="7b8bb-139">ID de processo (PID) do processo que modificou a chave de registro (os detalhes do processo aparecerão na coleção Alert ' Processes ').</span><span class="sxs-lookup"><span data-stu-id="7b8bb-139">Process ID (PID) of the process that modified the registry key (process details will appear in the alert 'processes' collection).</span></span>|
|<span data-ttu-id="7b8bb-140">valueData</span><span class="sxs-lookup"><span data-stu-id="7b8bb-140">valueData</span></span>|<span data-ttu-id="7b8bb-141">String</span><span class="sxs-lookup"><span data-stu-id="7b8bb-141">String</span></span>|<span data-ttu-id="7b8bb-142">Dados de valores de chave de registro (conteúdo) atuais (ou seja, alterados).</span><span class="sxs-lookup"><span data-stu-id="7b8bb-142">Current (i.e. changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="7b8bb-143">valueName</span><span class="sxs-lookup"><span data-stu-id="7b8bb-143">valueName</span></span>|<span data-ttu-id="7b8bb-144">String</span><span class="sxs-lookup"><span data-stu-id="7b8bb-144">String</span></span>|<span data-ttu-id="7b8bb-145">Nome do valor da chave do registro atual (ou seja, alterado)</span><span class="sxs-lookup"><span data-stu-id="7b8bb-145">Current (i.e. changed) registry key value name</span></span>|
|<span data-ttu-id="7b8bb-146">valueType</span><span class="sxs-lookup"><span data-stu-id="7b8bb-146">valueType</span></span>|<span data-ttu-id="7b8bb-147">registryValueType</span><span class="sxs-lookup"><span data-stu-id="7b8bb-147">registryValueType</span></span>|[<span data-ttu-id="7b8bb-148">Tipo de valor da chave do registro</span><span class="sxs-lookup"><span data-stu-id="7b8bb-148">Registry key value type</span></span>](/windows/desktop/sysinfo/registry-value-types) <ul><li><span data-ttu-id="7b8bb-149">REG_BINARY</span><span class="sxs-lookup"><span data-stu-id="7b8bb-149">REG_BINARY</span></span></li> <li><span data-ttu-id="7b8bb-150">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="7b8bb-150">REG_DWORD</span></span></li> <li><span data-ttu-id="7b8bb-151">REG_DWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="7b8bb-151">REG_DWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="7b8bb-152">REG_DWORD_BIG_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="7b8bb-152">REG_DWORD_BIG_ENDIAN</span></span></li><li><span data-ttu-id="7b8bb-153">REG_EXPAND_SZ</span><span class="sxs-lookup"><span data-stu-id="7b8bb-153">REG_EXPAND_SZ</span></span></li> <li><span data-ttu-id="7b8bb-154">REG_LINK</span><span class="sxs-lookup"><span data-stu-id="7b8bb-154">REG_LINK</span></span></li> <li><span data-ttu-id="7b8bb-155">REG_MULTI_SZ</span><span class="sxs-lookup"><span data-stu-id="7b8bb-155">REG_MULTI_SZ</span></span></li> <li><span data-ttu-id="7b8bb-156">REG_NONE</span><span class="sxs-lookup"><span data-stu-id="7b8bb-156">REG_NONE</span></span></li> <li><span data-ttu-id="7b8bb-157">REG_QWORD</span><span class="sxs-lookup"><span data-stu-id="7b8bb-157">REG_QWORD</span></span></li> <li><span data-ttu-id="7b8bb-158">REG_QWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="7b8bb-158">REG_QWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="7b8bb-159">REG_SZ</span><span class="sxs-lookup"><span data-stu-id="7b8bb-159">REG_SZ</span></span></li></ul> <span data-ttu-id="7b8bb-160">Os valores possíveis são: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.</span><span class="sxs-lookup"><span data-stu-id="7b8bb-160">Possible values are: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7b8bb-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b8bb-161">JSON representation</span></span>

<span data-ttu-id="7b8bb-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7b8bb-162">The following is a JSON representation of the resource.</span></span>

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
