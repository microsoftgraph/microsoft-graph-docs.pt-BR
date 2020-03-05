---
title: tipo de recurso registryKeystate
description: Contém informações sobre as alterações da chave do registro relacionadas ao alerta e o processo que alterou as chaves do registro.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 8f8f5aa0458666dfc10c4a3066534ea66821fb3a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521191"
---
# <a name="registrykeystate-resource-type"></a><span data-ttu-id="d83ac-103">tipo de recurso registryKeystate</span><span class="sxs-lookup"><span data-stu-id="d83ac-103">registryKeyState resource type</span></span>

<span data-ttu-id="d83ac-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d83ac-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d83ac-105">Contém informações sobre as alterações da chave do registro relacionadas ao alerta e o processo que alterou as chaves do registro.</span><span class="sxs-lookup"><span data-stu-id="d83ac-105">Contains information about registry key changes related to the alert, and the process that changed the registry keys.</span></span>

## <a name="properties"></a><span data-ttu-id="d83ac-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d83ac-106">Properties</span></span>

| <span data-ttu-id="d83ac-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d83ac-107">Property</span></span>     | <span data-ttu-id="d83ac-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d83ac-108">Type</span></span>        | <span data-ttu-id="d83ac-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d83ac-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d83ac-110">Hive</span><span class="sxs-lookup"><span data-stu-id="d83ac-110">hive</span></span>|<span data-ttu-id="d83ac-111">registryHive</span><span class="sxs-lookup"><span data-stu-id="d83ac-111">registryHive</span></span>|<span data-ttu-id="d83ac-112">Uma [seção de registro do Windows](/windows/desktop/sysinfo/registry-hives) :</span><span class="sxs-lookup"><span data-stu-id="d83ac-112">A [Windows registry hive](/windows/desktop/sysinfo/registry-hives) :</span></span> <ul><li><span data-ttu-id="d83ac-113">HKEY_CURRENT_CONFIG</span><span class="sxs-lookup"><span data-stu-id="d83ac-113">HKEY_CURRENT_CONFIG</span></span></li> <li><span data-ttu-id="d83ac-114">HKEY_CURRENT_USER</span><span class="sxs-lookup"><span data-stu-id="d83ac-114">HKEY_CURRENT_USER</span></span></li> <li><span data-ttu-id="d83ac-115">HKEY_LOCAL_MACHINE \SAM</span><span class="sxs-lookup"><span data-stu-id="d83ac-115">HKEY_LOCAL_MACHINE\SAM</span></span></li> <li><span data-ttu-id="d83ac-116">HKEY_LOCAL_MACHINE \Security</span><span class="sxs-lookup"><span data-stu-id="d83ac-116">HKEY_LOCAL_MACHINE\Security</span></span></li> <li><span data-ttu-id="d83ac-117">HKEY_LOCAL_MACHINE \Software</span><span class="sxs-lookup"><span data-stu-id="d83ac-117">HKEY_LOCAL_MACHINE\Software</span></span></li> <li><span data-ttu-id="d83ac-118">HKEY_LOCAL_MACHINE \System</span><span class="sxs-lookup"><span data-stu-id="d83ac-118">HKEY_LOCAL_MACHINE\System</span></span></li> <li><span data-ttu-id="d83ac-119">HKEY_USERS\\. Será.</span><span class="sxs-lookup"><span data-stu-id="d83ac-119">HKEY_USERS\\.Default.</span></span></li></ul> <span data-ttu-id="d83ac-120">Os valores possíveis são: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSecurity`, `localMachineSoftware`, `localMachineSystem`, `usersDefault`.</span><span class="sxs-lookup"><span data-stu-id="d83ac-120">Possible values are: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSecurity`, `localMachineSoftware`, `localMachineSystem`, `usersDefault`.</span></span>|
|<span data-ttu-id="d83ac-121">chave</span><span class="sxs-lookup"><span data-stu-id="d83ac-121">key</span></span>|<span data-ttu-id="d83ac-122">String</span><span class="sxs-lookup"><span data-stu-id="d83ac-122">String</span></span>|<span data-ttu-id="d83ac-123">Chave de registro atual (ou seja, alterada) (exclui HIVE).</span><span class="sxs-lookup"><span data-stu-id="d83ac-123">Current (i.e. changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="d83ac-124">oldKey</span><span class="sxs-lookup"><span data-stu-id="d83ac-124">oldKey</span></span>|<span data-ttu-id="d83ac-125">String</span><span class="sxs-lookup"><span data-stu-id="d83ac-125">String</span></span>|<span data-ttu-id="d83ac-126">Chave de registro anterior (ou seja, antes da alteração) (exclui HIVE).</span><span class="sxs-lookup"><span data-stu-id="d83ac-126">Previous (i.e. before changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="d83ac-127">oldValueData</span><span class="sxs-lookup"><span data-stu-id="d83ac-127">oldValueData</span></span>|<span data-ttu-id="d83ac-128">String</span><span class="sxs-lookup"><span data-stu-id="d83ac-128">String</span></span>|<span data-ttu-id="d83ac-129">Dados anteriores (ou seja, antes da alteração) dos valores da chave do registro (conteúdo).</span><span class="sxs-lookup"><span data-stu-id="d83ac-129">Previous (i.e. before changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="d83ac-130">oldValue</span><span class="sxs-lookup"><span data-stu-id="d83ac-130">oldValueName</span></span>|<span data-ttu-id="d83ac-131">String</span><span class="sxs-lookup"><span data-stu-id="d83ac-131">String</span></span>|<span data-ttu-id="d83ac-132">Nome do valor da chave anterior (ou seja, antes da alteração).</span><span class="sxs-lookup"><span data-stu-id="d83ac-132">Previous (i.e. before changed) registry key value name.</span></span>|
|<span data-ttu-id="d83ac-133">operações</span><span class="sxs-lookup"><span data-stu-id="d83ac-133">operation</span></span>|<span data-ttu-id="d83ac-134">registryOperation</span><span class="sxs-lookup"><span data-stu-id="d83ac-134">registryOperation</span></span>|<span data-ttu-id="d83ac-135">Operação que alterou o nome da chave do registro e/ou o valor.</span><span class="sxs-lookup"><span data-stu-id="d83ac-135">Operation that changed the registry key name and/or value.</span></span> <span data-ttu-id="d83ac-136">Os valores possíveis são: `unknown`, `create`, `modify`, `delete`.</span><span class="sxs-lookup"><span data-stu-id="d83ac-136">Possible values are: `unknown`, `create`, `modify`, `delete`.</span></span>|
|<span data-ttu-id="d83ac-137">Identificação</span><span class="sxs-lookup"><span data-stu-id="d83ac-137">processId</span></span>|<span data-ttu-id="d83ac-138">Int32</span><span class="sxs-lookup"><span data-stu-id="d83ac-138">Int32</span></span>|<span data-ttu-id="d83ac-139">ID de processo (PID) do processo que modificou a chave de registro (os detalhes do processo aparecerão na coleção Alert ' Processes ').</span><span class="sxs-lookup"><span data-stu-id="d83ac-139">Process ID (PID) of the process that modified the registry key (process details will appear in the alert 'processes' collection).</span></span>|
|<span data-ttu-id="d83ac-140">valueData</span><span class="sxs-lookup"><span data-stu-id="d83ac-140">valueData</span></span>|<span data-ttu-id="d83ac-141">String</span><span class="sxs-lookup"><span data-stu-id="d83ac-141">String</span></span>|<span data-ttu-id="d83ac-142">Dados de valores de chave de registro (conteúdo) atuais (ou seja, alterados).</span><span class="sxs-lookup"><span data-stu-id="d83ac-142">Current (i.e. changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="d83ac-143">valueName</span><span class="sxs-lookup"><span data-stu-id="d83ac-143">valueName</span></span>|<span data-ttu-id="d83ac-144">String</span><span class="sxs-lookup"><span data-stu-id="d83ac-144">String</span></span>|<span data-ttu-id="d83ac-145">Nome do valor da chave do registro atual (ou seja, alterado)</span><span class="sxs-lookup"><span data-stu-id="d83ac-145">Current (i.e. changed) registry key value name</span></span>|
|<span data-ttu-id="d83ac-146">valueType</span><span class="sxs-lookup"><span data-stu-id="d83ac-146">valueType</span></span>|<span data-ttu-id="d83ac-147">registryValueType</span><span class="sxs-lookup"><span data-stu-id="d83ac-147">registryValueType</span></span>|[<span data-ttu-id="d83ac-148">Tipo de valor da chave do registro</span><span class="sxs-lookup"><span data-stu-id="d83ac-148">Registry key value type</span></span>](/windows/desktop/sysinfo/registry-value-types) <ul><li><span data-ttu-id="d83ac-149">REG_BINARY</span><span class="sxs-lookup"><span data-stu-id="d83ac-149">REG_BINARY</span></span></li> <li><span data-ttu-id="d83ac-150">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="d83ac-150">REG_DWORD</span></span></li> <li><span data-ttu-id="d83ac-151">REG_DWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="d83ac-151">REG_DWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="d83ac-152">REG_DWORD_BIG_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="d83ac-152">REG_DWORD_BIG_ENDIAN</span></span></li><li><span data-ttu-id="d83ac-153">REG_EXPAND_SZ</span><span class="sxs-lookup"><span data-stu-id="d83ac-153">REG_EXPAND_SZ</span></span></li> <li><span data-ttu-id="d83ac-154">REG_LINK</span><span class="sxs-lookup"><span data-stu-id="d83ac-154">REG_LINK</span></span></li> <li><span data-ttu-id="d83ac-155">REG_MULTI_SZ</span><span class="sxs-lookup"><span data-stu-id="d83ac-155">REG_MULTI_SZ</span></span></li> <li><span data-ttu-id="d83ac-156">REG_NONE</span><span class="sxs-lookup"><span data-stu-id="d83ac-156">REG_NONE</span></span></li> <li><span data-ttu-id="d83ac-157">REG_QWORD</span><span class="sxs-lookup"><span data-stu-id="d83ac-157">REG_QWORD</span></span></li> <li><span data-ttu-id="d83ac-158">REG_QWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="d83ac-158">REG_QWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="d83ac-159">REG_SZ</span><span class="sxs-lookup"><span data-stu-id="d83ac-159">REG_SZ</span></span></li></ul> <span data-ttu-id="d83ac-160">Os valores possíveis são: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.</span><span class="sxs-lookup"><span data-stu-id="d83ac-160">Possible values are: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d83ac-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d83ac-161">JSON representation</span></span>

<span data-ttu-id="d83ac-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d83ac-162">The following is a JSON representation of the resource.</span></span>

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
