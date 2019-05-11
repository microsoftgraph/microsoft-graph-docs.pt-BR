---
title: Criar windowsInformationProtectionAppLockerFile
description: Criar um novo objeto windowsInformationProtectionAppLockerFile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ad14be8ae66c48a66899d9ab8c5590d847aa7a77
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33902959"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="ba1bd-103">Criar windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="ba1bd-103">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="ba1bd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ba1bd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba1bd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ba1bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba1bd-106">Criar um novo objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="ba1bd-106">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba1bd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ba1bd-107">Prerequisites</span></span>
<span data-ttu-id="ba1bd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba1bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba1bd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba1bd-110">Permission type</span></span>|<span data-ttu-id="ba1bd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ba1bd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba1bd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba1bd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ba1bd-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba1bd-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ba1bd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba1bd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba1bd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba1bd-115">Not supported.</span></span>|
|<span data-ttu-id="ba1bd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba1bd-116">Application</span></span>|<span data-ttu-id="ba1bd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba1bd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba1bd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba1bd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
POST /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles
```

## <a name="request-headers"></a><span data-ttu-id="ba1bd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba1bd-119">Request headers</span></span>
|<span data-ttu-id="ba1bd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ba1bd-120">Header</span></span>|<span data-ttu-id="ba1bd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ba1bd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba1bd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba1bd-122">Authorization</span></span>|<span data-ttu-id="ba1bd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba1bd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba1bd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ba1bd-124">Accept</span></span>|<span data-ttu-id="ba1bd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ba1bd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba1bd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba1bd-126">Request body</span></span>
<span data-ttu-id="ba1bd-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionAppLockerFile.</span><span class="sxs-lookup"><span data-stu-id="ba1bd-127">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="ba1bd-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionAppLockerFile.</span><span class="sxs-lookup"><span data-stu-id="ba1bd-128">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="ba1bd-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba1bd-129">Property</span></span>|<span data-ttu-id="ba1bd-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba1bd-130">Type</span></span>|<span data-ttu-id="ba1bd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba1bd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba1bd-132">displayName</span><span class="sxs-lookup"><span data-stu-id="ba1bd-132">displayName</span></span>|<span data-ttu-id="ba1bd-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba1bd-133">String</span></span>|<span data-ttu-id="ba1bd-134">O nome amigável</span><span class="sxs-lookup"><span data-stu-id="ba1bd-134">The friendly name</span></span>|
|<span data-ttu-id="ba1bd-135">fileHash</span><span class="sxs-lookup"><span data-stu-id="ba1bd-135">fileHash</span></span>|<span data-ttu-id="ba1bd-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba1bd-136">String</span></span>|<span data-ttu-id="ba1bd-137">Hash SHA256 do arquivo</span><span class="sxs-lookup"><span data-stu-id="ba1bd-137">SHA256 hash of the file</span></span>|
|<span data-ttu-id="ba1bd-138">file</span><span class="sxs-lookup"><span data-stu-id="ba1bd-138">file</span></span>|<span data-ttu-id="ba1bd-139">Binária</span><span class="sxs-lookup"><span data-stu-id="ba1bd-139">Binary</span></span>|<span data-ttu-id="ba1bd-140">Arquivo como uma matriz de bytes</span><span class="sxs-lookup"><span data-stu-id="ba1bd-140">File as a byte array</span></span>|
|<span data-ttu-id="ba1bd-141">id</span><span class="sxs-lookup"><span data-stu-id="ba1bd-141">id</span></span>|<span data-ttu-id="ba1bd-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba1bd-142">String</span></span>|<span data-ttu-id="ba1bd-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ba1bd-143">Key of the entity.</span></span>|
|<span data-ttu-id="ba1bd-144">versão</span><span class="sxs-lookup"><span data-stu-id="ba1bd-144">version</span></span>|<span data-ttu-id="ba1bd-145">String</span><span class="sxs-lookup"><span data-stu-id="ba1bd-145">String</span></span>|<span data-ttu-id="ba1bd-146">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="ba1bd-146">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="ba1bd-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba1bd-147">Response</span></span>
<span data-ttu-id="ba1bd-148">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba1bd-148">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba1bd-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ba1bd-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba1bd-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba1bd-150">Request</span></span>
<span data-ttu-id="ba1bd-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba1bd-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
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

### <a name="response"></a><span data-ttu-id="ba1bd-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba1bd-152">Response</span></span>
<span data-ttu-id="ba1bd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ba1bd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




