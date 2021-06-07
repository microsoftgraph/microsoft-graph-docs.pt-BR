---
title: Atualizar windowsInformationProtectionAppLockerFile
description: Atualizar as propriedades de um objeto windowsInformationProtectionAppLockerFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 373e7066bd78c9997a7170399bc23ffcab3e6765
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759090"
---
# <a name="update-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="dbe8b-103">Atualizar windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="dbe8b-103">Update windowsInformationProtectionAppLockerFile</span></span>

<span data-ttu-id="dbe8b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbe8b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dbe8b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dbe8b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbe8b-106">Atualizar as propriedades de um objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="dbe8b-106">Update the properties of a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dbe8b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dbe8b-107">Prerequisites</span></span>
<span data-ttu-id="dbe8b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbe8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbe8b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dbe8b-110">Permission type</span></span>|<span data-ttu-id="dbe8b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dbe8b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dbe8b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dbe8b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dbe8b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbe8b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dbe8b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dbe8b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dbe8b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbe8b-115">Not supported.</span></span>|
|<span data-ttu-id="dbe8b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dbe8b-116">Application</span></span>|<span data-ttu-id="dbe8b-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbe8b-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dbe8b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dbe8b-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="dbe8b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dbe8b-119">Request headers</span></span>
|<span data-ttu-id="dbe8b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dbe8b-120">Header</span></span>|<span data-ttu-id="dbe8b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="dbe8b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dbe8b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dbe8b-122">Authorization</span></span>|<span data-ttu-id="dbe8b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dbe8b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dbe8b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dbe8b-124">Accept</span></span>|<span data-ttu-id="dbe8b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dbe8b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbe8b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dbe8b-126">Request body</span></span>
<span data-ttu-id="dbe8b-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="dbe8b-127">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

<span data-ttu-id="dbe8b-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="dbe8b-128">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span></span>

|<span data-ttu-id="dbe8b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dbe8b-129">Property</span></span>|<span data-ttu-id="dbe8b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbe8b-130">Type</span></span>|<span data-ttu-id="dbe8b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbe8b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbe8b-132">displayName</span><span class="sxs-lookup"><span data-stu-id="dbe8b-132">displayName</span></span>|<span data-ttu-id="dbe8b-133">String</span><span class="sxs-lookup"><span data-stu-id="dbe8b-133">String</span></span>|<span data-ttu-id="dbe8b-134">O nome amigável</span><span class="sxs-lookup"><span data-stu-id="dbe8b-134">The friendly name</span></span>|
|<span data-ttu-id="dbe8b-135">fileHash</span><span class="sxs-lookup"><span data-stu-id="dbe8b-135">fileHash</span></span>|<span data-ttu-id="dbe8b-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbe8b-136">String</span></span>|<span data-ttu-id="dbe8b-137">Hash SHA256 do arquivo</span><span class="sxs-lookup"><span data-stu-id="dbe8b-137">SHA256 hash of the file</span></span>|
|<span data-ttu-id="dbe8b-138">file</span><span class="sxs-lookup"><span data-stu-id="dbe8b-138">file</span></span>|<span data-ttu-id="dbe8b-139">Binária</span><span class="sxs-lookup"><span data-stu-id="dbe8b-139">Binary</span></span>|<span data-ttu-id="dbe8b-140">Arquivo como uma matriz de bytes</span><span class="sxs-lookup"><span data-stu-id="dbe8b-140">File as a byte array</span></span>|
|<span data-ttu-id="dbe8b-141">id</span><span class="sxs-lookup"><span data-stu-id="dbe8b-141">id</span></span>|<span data-ttu-id="dbe8b-142">String</span><span class="sxs-lookup"><span data-stu-id="dbe8b-142">String</span></span>|<span data-ttu-id="dbe8b-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="dbe8b-143">Key of the entity.</span></span>|
|<span data-ttu-id="dbe8b-144">versão</span><span class="sxs-lookup"><span data-stu-id="dbe8b-144">version</span></span>|<span data-ttu-id="dbe8b-145">String</span><span class="sxs-lookup"><span data-stu-id="dbe8b-145">String</span></span>|<span data-ttu-id="dbe8b-146">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="dbe8b-146">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="dbe8b-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbe8b-147">Response</span></span>
<span data-ttu-id="dbe8b-148">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dbe8b-148">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbe8b-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dbe8b-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="dbe8b-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dbe8b-150">Request</span></span>
<span data-ttu-id="dbe8b-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dbe8b-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dbe8b-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbe8b-152">Response</span></span>
<span data-ttu-id="dbe8b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dbe8b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




