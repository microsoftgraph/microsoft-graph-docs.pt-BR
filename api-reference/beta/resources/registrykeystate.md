---
title: tipo de recurso registryKeystate
description: Contém informações sobre as alterações da chave do registro relacionadas ao alerta e o processo que alterou as chaves do registro.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: e685bc281344f05a43e3c44b7df6bb6884185c63
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870128"
---
# <a name="registrykeystate-resource-type"></a><span data-ttu-id="ac003-103">tipo de recurso registryKeystate</span><span class="sxs-lookup"><span data-stu-id="ac003-103">registryKeyState resource type</span></span>

<span data-ttu-id="ac003-104">Contém informações sobre as alterações da chave do registro relacionadas ao alerta e o processo que alterou as chaves do registro.</span><span class="sxs-lookup"><span data-stu-id="ac003-104">Contains information about registry key changes related to the alert, and the process that changed the registry keys.</span></span>

## <a name="properties"></a><span data-ttu-id="ac003-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ac003-105">Properties</span></span>

| <span data-ttu-id="ac003-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac003-106">Property</span></span>     | <span data-ttu-id="ac003-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac003-107">Type</span></span>        | <span data-ttu-id="ac003-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac003-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ac003-109">Hive</span><span class="sxs-lookup"><span data-stu-id="ac003-109">hive</span></span>|<span data-ttu-id="ac003-110">registryHive</span><span class="sxs-lookup"><span data-stu-id="ac003-110">registryHive</span></span>|<span data-ttu-id="ac003-111">Uma [seção de registro do Windows](/windows/desktop/sysinfo/registry-hives) :</span><span class="sxs-lookup"><span data-stu-id="ac003-111">A [Windows registry hive](/windows/desktop/sysinfo/registry-hives) :</span></span> <ul><li><span data-ttu-id="ac003-112">HKEY_CURRENT_CONFIG</span><span class="sxs-lookup"><span data-stu-id="ac003-112">HKEY_CURRENT_CONFIG</span></span></li> <li><span data-ttu-id="ac003-113">HKEY_CURRENT_USER</span><span class="sxs-lookup"><span data-stu-id="ac003-113">HKEY_CURRENT_USER</span></span></li> <li><span data-ttu-id="ac003-114">HKEY_LOCAL_MACHINE \SAM</span><span class="sxs-lookup"><span data-stu-id="ac003-114">HKEY_LOCAL_MACHINE\SAM</span></span></li> <li><span data-ttu-id="ac003-115">HKEY_LOCAL_MACHINE \Security</span><span class="sxs-lookup"><span data-stu-id="ac003-115">HKEY_LOCAL_MACHINE\Security</span></span></li> <li><span data-ttu-id="ac003-116">HKEY_LOCAL_MACHINE \Software</span><span class="sxs-lookup"><span data-stu-id="ac003-116">HKEY_LOCAL_MACHINE\Software</span></span></li> <li><span data-ttu-id="ac003-117">HKEY_LOCAL_MACHINE \System</span><span class="sxs-lookup"><span data-stu-id="ac003-117">HKEY_LOCAL_MACHINE\System</span></span></li> <li><span data-ttu-id="ac003-118">HKEY_USERS\\. Será.</span><span class="sxs-lookup"><span data-stu-id="ac003-118">HKEY_USERS\\.Default.</span></span></li></ul> <span data-ttu-id="ac003-119">Os valores possíveis são: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSecurity`, `localMachineSoftware`, `localMachineSystem`, `usersDefault`.</span><span class="sxs-lookup"><span data-stu-id="ac003-119">Possible values are: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSecurity`, `localMachineSoftware`, `localMachineSystem`, `usersDefault`.</span></span>|
|<span data-ttu-id="ac003-120">chave</span><span class="sxs-lookup"><span data-stu-id="ac003-120">key</span></span>|<span data-ttu-id="ac003-121">String</span><span class="sxs-lookup"><span data-stu-id="ac003-121">String</span></span>|<span data-ttu-id="ac003-122">Chave de registro atual (ou seja, alterada) (exclui HIVE).</span><span class="sxs-lookup"><span data-stu-id="ac003-122">Current (i.e. changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="ac003-123">oldKey</span><span class="sxs-lookup"><span data-stu-id="ac003-123">oldKey</span></span>|<span data-ttu-id="ac003-124">String</span><span class="sxs-lookup"><span data-stu-id="ac003-124">String</span></span>|<span data-ttu-id="ac003-125">Chave de registro anterior (ou seja, antes da alteração) (exclui HIVE).</span><span class="sxs-lookup"><span data-stu-id="ac003-125">Previous (i.e. before changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="ac003-126">oldValueData</span><span class="sxs-lookup"><span data-stu-id="ac003-126">oldValueData</span></span>|<span data-ttu-id="ac003-127">String</span><span class="sxs-lookup"><span data-stu-id="ac003-127">String</span></span>|<span data-ttu-id="ac003-128">Dados anteriores (ou seja, antes da alteração) dos valores da chave do registro (conteúdo).</span><span class="sxs-lookup"><span data-stu-id="ac003-128">Previous (i.e. before changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="ac003-129">oldValue</span><span class="sxs-lookup"><span data-stu-id="ac003-129">oldValueName</span></span>|<span data-ttu-id="ac003-130">String</span><span class="sxs-lookup"><span data-stu-id="ac003-130">String</span></span>|<span data-ttu-id="ac003-131">Nome do valor da chave anterior (ou seja, antes da alteração).</span><span class="sxs-lookup"><span data-stu-id="ac003-131">Previous (i.e. before changed) registry key value name.</span></span>|
|<span data-ttu-id="ac003-132">operações</span><span class="sxs-lookup"><span data-stu-id="ac003-132">operation</span></span>|<span data-ttu-id="ac003-133">registryOperation</span><span class="sxs-lookup"><span data-stu-id="ac003-133">registryOperation</span></span>|<span data-ttu-id="ac003-134">Operação que alterou o nome da chave do registro e/ou o valor.</span><span class="sxs-lookup"><span data-stu-id="ac003-134">Operation that changed the registry key name and/or value.</span></span> <span data-ttu-id="ac003-135">Os valores possíveis são: `unknown`, `create`, `modify`, `delete`.</span><span class="sxs-lookup"><span data-stu-id="ac003-135">Possible values are: `unknown`, `create`, `modify`, `delete`.</span></span>|
|<span data-ttu-id="ac003-136">Identificação</span><span class="sxs-lookup"><span data-stu-id="ac003-136">processId</span></span>|<span data-ttu-id="ac003-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ac003-137">Int32</span></span>|<span data-ttu-id="ac003-138">ID de processo (PID) do processo que modificou a chave de registro (os detalhes do processo aparecerão na coleção Alert ' Processes ').</span><span class="sxs-lookup"><span data-stu-id="ac003-138">Process ID (PID) of the process that modified the registry key (process details will appear in the alert 'processes' collection).</span></span>|
|<span data-ttu-id="ac003-139">valueData</span><span class="sxs-lookup"><span data-stu-id="ac003-139">valueData</span></span>|<span data-ttu-id="ac003-140">String</span><span class="sxs-lookup"><span data-stu-id="ac003-140">String</span></span>|<span data-ttu-id="ac003-141">Dados de valores de chave de registro (conteúdo) atuais (ou seja, alterados).</span><span class="sxs-lookup"><span data-stu-id="ac003-141">Current (i.e. changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="ac003-142">valueName</span><span class="sxs-lookup"><span data-stu-id="ac003-142">valueName</span></span>|<span data-ttu-id="ac003-143">String</span><span class="sxs-lookup"><span data-stu-id="ac003-143">String</span></span>|<span data-ttu-id="ac003-144">Nome do valor da chave do registro atual (ou seja, alterado)</span><span class="sxs-lookup"><span data-stu-id="ac003-144">Current (i.e. changed) registry key value name</span></span>|
|<span data-ttu-id="ac003-145">valueType</span><span class="sxs-lookup"><span data-stu-id="ac003-145">valueType</span></span>|<span data-ttu-id="ac003-146">registryValueType</span><span class="sxs-lookup"><span data-stu-id="ac003-146">registryValueType</span></span>|[<span data-ttu-id="ac003-147">Tipo de valor da chave do registro</span><span class="sxs-lookup"><span data-stu-id="ac003-147">Registry key value type</span></span>](/windows/desktop/sysinfo/registry-value-types) <ul><li><span data-ttu-id="ac003-148">REG_BINARY</span><span class="sxs-lookup"><span data-stu-id="ac003-148">REG_BINARY</span></span></li> <li><span data-ttu-id="ac003-149">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="ac003-149">REG_DWORD</span></span></li> <li><span data-ttu-id="ac003-150">REG_DWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="ac003-150">REG_DWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="ac003-151">REG_DWORD_BIG_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="ac003-151">REG_DWORD_BIG_ENDIAN</span></span></li><li><span data-ttu-id="ac003-152">REG_EXPAND_SZ</span><span class="sxs-lookup"><span data-stu-id="ac003-152">REG_EXPAND_SZ</span></span></li> <li><span data-ttu-id="ac003-153">REG_LINK</span><span class="sxs-lookup"><span data-stu-id="ac003-153">REG_LINK</span></span></li> <li><span data-ttu-id="ac003-154">REG_MULTI_SZ</span><span class="sxs-lookup"><span data-stu-id="ac003-154">REG_MULTI_SZ</span></span></li> <li><span data-ttu-id="ac003-155">REG_NONE</span><span class="sxs-lookup"><span data-stu-id="ac003-155">REG_NONE</span></span></li> <li><span data-ttu-id="ac003-156">REG_QWORD</span><span class="sxs-lookup"><span data-stu-id="ac003-156">REG_QWORD</span></span></li> <li><span data-ttu-id="ac003-157">REG_QWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="ac003-157">REG_QWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="ac003-158">REG_SZ</span><span class="sxs-lookup"><span data-stu-id="ac003-158">REG_SZ</span></span></li></ul> <span data-ttu-id="ac003-159">Os valores possíveis são: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.</span><span class="sxs-lookup"><span data-stu-id="ac003-159">Possible values are: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ac003-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ac003-160">JSON representation</span></span>

<span data-ttu-id="ac003-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ac003-161">The following is a JSON representation of the resource.</span></span>

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
