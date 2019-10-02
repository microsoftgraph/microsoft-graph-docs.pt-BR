---
title: Atualizar windowsInformationProtectionAppLockerFile
description: Atualizar as propriedades de um objeto windowsInformationProtectionAppLockerFile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: acebebc6024846d62a4ece0cbd1173da34d710e6
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37362993"
---
# <a name="update-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="c30fb-103">Atualizar windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="c30fb-103">Update windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="c30fb-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c30fb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c30fb-105">Atualizar as propriedades de um objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="c30fb-105">Update the properties of a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c30fb-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c30fb-106">Prerequisites</span></span>
<span data-ttu-id="c30fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c30fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c30fb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c30fb-109">Permission type</span></span>|<span data-ttu-id="c30fb-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c30fb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c30fb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c30fb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c30fb-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c30fb-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c30fb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c30fb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c30fb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c30fb-114">Not supported.</span></span>|
|<span data-ttu-id="c30fb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c30fb-115">Application</span></span>|<span data-ttu-id="c30fb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c30fb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c30fb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c30fb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
```

## <a name="request-headers"></a><span data-ttu-id="c30fb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c30fb-118">Request headers</span></span>
|<span data-ttu-id="c30fb-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c30fb-119">Header</span></span>|<span data-ttu-id="c30fb-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c30fb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c30fb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c30fb-121">Authorization</span></span>|<span data-ttu-id="c30fb-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c30fb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c30fb-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c30fb-123">Accept</span></span>|<span data-ttu-id="c30fb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c30fb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c30fb-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c30fb-125">Request body</span></span>
<span data-ttu-id="c30fb-126">No corpo da solicitação, forneça uma representação JSON do objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="c30fb-126">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

<span data-ttu-id="c30fb-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="c30fb-127">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span></span>

|<span data-ttu-id="c30fb-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c30fb-128">Property</span></span>|<span data-ttu-id="c30fb-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="c30fb-129">Type</span></span>|<span data-ttu-id="c30fb-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="c30fb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c30fb-131">displayName</span><span class="sxs-lookup"><span data-stu-id="c30fb-131">displayName</span></span>|<span data-ttu-id="c30fb-132">String</span><span class="sxs-lookup"><span data-stu-id="c30fb-132">String</span></span>|<span data-ttu-id="c30fb-133">O nome amigável</span><span class="sxs-lookup"><span data-stu-id="c30fb-133">The friendly name</span></span>|
|<span data-ttu-id="c30fb-134">fileHash</span><span class="sxs-lookup"><span data-stu-id="c30fb-134">fileHash</span></span>|<span data-ttu-id="c30fb-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c30fb-135">String</span></span>|<span data-ttu-id="c30fb-136">Hash SHA256 do arquivo</span><span class="sxs-lookup"><span data-stu-id="c30fb-136">SHA256 hash of the file</span></span>|
|<span data-ttu-id="c30fb-137">file</span><span class="sxs-lookup"><span data-stu-id="c30fb-137">file</span></span>|<span data-ttu-id="c30fb-138">Binária</span><span class="sxs-lookup"><span data-stu-id="c30fb-138">Binary</span></span>|<span data-ttu-id="c30fb-139">Arquivo como uma matriz de bytes</span><span class="sxs-lookup"><span data-stu-id="c30fb-139">File as a byte array</span></span>|
|<span data-ttu-id="c30fb-140">id</span><span class="sxs-lookup"><span data-stu-id="c30fb-140">id</span></span>|<span data-ttu-id="c30fb-141">String</span><span class="sxs-lookup"><span data-stu-id="c30fb-141">String</span></span>|<span data-ttu-id="c30fb-142">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c30fb-142">Key of the entity.</span></span>|
|<span data-ttu-id="c30fb-143">versão</span><span class="sxs-lookup"><span data-stu-id="c30fb-143">version</span></span>|<span data-ttu-id="c30fb-144">String</span><span class="sxs-lookup"><span data-stu-id="c30fb-144">String</span></span>|<span data-ttu-id="c30fb-145">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="c30fb-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="c30fb-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="c30fb-146">Response</span></span>
<span data-ttu-id="c30fb-147">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c30fb-147">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c30fb-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c30fb-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="c30fb-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c30fb-149">Request</span></span>
<span data-ttu-id="c30fb-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c30fb-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="c30fb-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="c30fb-151">Response</span></span>
<span data-ttu-id="c30fb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c30fb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "id": "d81f0e40-0e40-d81f-400e-1fd8400e1fd8",
  "version": "Version value"
}
```




