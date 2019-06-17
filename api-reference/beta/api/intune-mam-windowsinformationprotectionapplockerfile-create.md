---
title: Criar windowsInformationProtectionAppLockerFile
description: Criar um novo objeto windowsInformationProtectionAppLockerFile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0d5393fdbf68de218cd146817f68afbd125fa70d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987429"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="56280-103">Criar windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="56280-103">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="56280-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="56280-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56280-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="56280-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56280-106">Criar um novo objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="56280-106">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="56280-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="56280-107">Prerequisites</span></span>
<span data-ttu-id="56280-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56280-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56280-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56280-110">Permission type</span></span>|<span data-ttu-id="56280-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="56280-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56280-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56280-112">Delegated (work or school account)</span></span>|<span data-ttu-id="56280-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56280-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="56280-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56280-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56280-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56280-115">Not supported.</span></span>|
|<span data-ttu-id="56280-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56280-116">Application</span></span>|<span data-ttu-id="56280-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56280-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56280-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56280-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="56280-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56280-119">Request headers</span></span>
|<span data-ttu-id="56280-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="56280-120">Header</span></span>|<span data-ttu-id="56280-121">Valor</span><span class="sxs-lookup"><span data-stu-id="56280-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56280-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="56280-122">Authorization</span></span>|<span data-ttu-id="56280-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56280-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56280-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="56280-124">Accept</span></span>|<span data-ttu-id="56280-125">application/json</span><span class="sxs-lookup"><span data-stu-id="56280-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56280-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56280-126">Request body</span></span>
<span data-ttu-id="56280-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionAppLockerFile.</span><span class="sxs-lookup"><span data-stu-id="56280-127">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="56280-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionAppLockerFile.</span><span class="sxs-lookup"><span data-stu-id="56280-128">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="56280-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56280-129">Property</span></span>|<span data-ttu-id="56280-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="56280-130">Type</span></span>|<span data-ttu-id="56280-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="56280-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56280-132">displayName</span><span class="sxs-lookup"><span data-stu-id="56280-132">displayName</span></span>|<span data-ttu-id="56280-133">String</span><span class="sxs-lookup"><span data-stu-id="56280-133">String</span></span>|<span data-ttu-id="56280-134">O nome amigável</span><span class="sxs-lookup"><span data-stu-id="56280-134">The friendly name</span></span>|
|<span data-ttu-id="56280-135">fileHash</span><span class="sxs-lookup"><span data-stu-id="56280-135">fileHash</span></span>|<span data-ttu-id="56280-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="56280-136">String</span></span>|<span data-ttu-id="56280-137">Hash SHA256 do arquivo</span><span class="sxs-lookup"><span data-stu-id="56280-137">SHA256 hash of the file</span></span>|
|<span data-ttu-id="56280-138">file</span><span class="sxs-lookup"><span data-stu-id="56280-138">file</span></span>|<span data-ttu-id="56280-139">Binária</span><span class="sxs-lookup"><span data-stu-id="56280-139">Binary</span></span>|<span data-ttu-id="56280-140">Arquivo como uma matriz de bytes</span><span class="sxs-lookup"><span data-stu-id="56280-140">File as a byte array</span></span>|
|<span data-ttu-id="56280-141">id</span><span class="sxs-lookup"><span data-stu-id="56280-141">id</span></span>|<span data-ttu-id="56280-142">String</span><span class="sxs-lookup"><span data-stu-id="56280-142">String</span></span>|<span data-ttu-id="56280-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="56280-143">Key of the entity.</span></span>|
|<span data-ttu-id="56280-144">versão</span><span class="sxs-lookup"><span data-stu-id="56280-144">version</span></span>|<span data-ttu-id="56280-145">String</span><span class="sxs-lookup"><span data-stu-id="56280-145">String</span></span>|<span data-ttu-id="56280-146">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="56280-146">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="56280-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="56280-147">Response</span></span>
<span data-ttu-id="56280-148">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56280-148">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56280-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56280-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="56280-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56280-150">Request</span></span>
<span data-ttu-id="56280-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="56280-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="56280-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="56280-152">Response</span></span>
<span data-ttu-id="56280-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="56280-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





