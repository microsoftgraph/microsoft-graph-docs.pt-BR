---
title: Criar windowsInformationProtectionAppLockerFile
description: Criar um novo objeto windowsInformationProtectionAppLockerFile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 13b6d9a0e8fc6e23b2a5b7b85e257ef8d3ac9c34
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853316"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="b8d6d-103">Criar windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="b8d6d-103">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="b8d6d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b8d6d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8d6d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b8d6d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b8d6d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b8d6d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8d6d-107">Criar um novo objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="b8d6d-107">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b8d6d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b8d6d-108">Prerequisites</span></span>
<span data-ttu-id="b8d6d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8d6d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8d6d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8d6d-111">Permission type</span></span>|<span data-ttu-id="b8d6d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b8d6d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8d6d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8d6d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b8d6d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8d6d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b8d6d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8d6d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8d6d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8d6d-116">Not supported.</span></span>|
|<span data-ttu-id="b8d6d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8d6d-117">Application</span></span>|<span data-ttu-id="b8d6d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8d6d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8d6d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8d6d-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="b8d6d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8d6d-120">Request headers</span></span>
|<span data-ttu-id="b8d6d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b8d6d-121">Header</span></span>|<span data-ttu-id="b8d6d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b8d6d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8d6d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8d6d-123">Authorization</span></span>|<span data-ttu-id="b8d6d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8d6d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8d6d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b8d6d-125">Accept</span></span>|<span data-ttu-id="b8d6d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b8d6d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8d6d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8d6d-127">Request body</span></span>
<span data-ttu-id="b8d6d-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionAppLockerFile.</span><span class="sxs-lookup"><span data-stu-id="b8d6d-128">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="b8d6d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionAppLockerFile.</span><span class="sxs-lookup"><span data-stu-id="b8d6d-129">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="b8d6d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b8d6d-130">Property</span></span>|<span data-ttu-id="b8d6d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8d6d-131">Type</span></span>|<span data-ttu-id="b8d6d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8d6d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8d6d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="b8d6d-133">displayName</span></span>|<span data-ttu-id="b8d6d-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8d6d-134">String</span></span>|<span data-ttu-id="b8d6d-135">O nome amigável</span><span class="sxs-lookup"><span data-stu-id="b8d6d-135">The friendly name</span></span>|
|<span data-ttu-id="b8d6d-136">fileHash</span><span class="sxs-lookup"><span data-stu-id="b8d6d-136">fileHash</span></span>|<span data-ttu-id="b8d6d-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8d6d-137">String</span></span>|<span data-ttu-id="b8d6d-138">Hash SHA256 do arquivo</span><span class="sxs-lookup"><span data-stu-id="b8d6d-138">SHA256 hash of the file</span></span>|
|<span data-ttu-id="b8d6d-139">file</span><span class="sxs-lookup"><span data-stu-id="b8d6d-139">file</span></span>|<span data-ttu-id="b8d6d-140">Binária</span><span class="sxs-lookup"><span data-stu-id="b8d6d-140">Binary</span></span>|<span data-ttu-id="b8d6d-141">Arquivo como uma matriz de bytes</span><span class="sxs-lookup"><span data-stu-id="b8d6d-141">File as a byte array</span></span>|
|<span data-ttu-id="b8d6d-142">id</span><span class="sxs-lookup"><span data-stu-id="b8d6d-142">id</span></span>|<span data-ttu-id="b8d6d-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8d6d-143">String</span></span>|<span data-ttu-id="b8d6d-144">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b8d6d-144">Key of the entity.</span></span>|
|<span data-ttu-id="b8d6d-145">version</span><span class="sxs-lookup"><span data-stu-id="b8d6d-145">version</span></span>|<span data-ttu-id="b8d6d-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8d6d-146">String</span></span>|<span data-ttu-id="b8d6d-147">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="b8d6d-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="b8d6d-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8d6d-148">Response</span></span>
<span data-ttu-id="b8d6d-149">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8d6d-149">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8d6d-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8d6d-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="b8d6d-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8d6d-151">Request</span></span>
<span data-ttu-id="b8d6d-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8d6d-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b8d6d-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8d6d-153">Response</span></span>
<span data-ttu-id="b8d6d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8d6d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





