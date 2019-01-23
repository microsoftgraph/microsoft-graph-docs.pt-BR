---
title: Criar windowsInformationProtectionAppLockerFile
description: Criar um novo objeto windowsInformationProtectionAppLockerFile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9d55359478d72df0001ac730f6fffed8c70af066
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414778"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="5dc56-103">Criar windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="5dc56-103">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="5dc56-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="5dc56-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5dc56-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5dc56-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5dc56-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="5dc56-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5dc56-107">Criar um novo objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="5dc56-107">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5dc56-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5dc56-108">Prerequisites</span></span>
<span data-ttu-id="5dc56-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5dc56-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5dc56-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5dc56-111">Permission type</span></span>|<span data-ttu-id="5dc56-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5dc56-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5dc56-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5dc56-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5dc56-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dc56-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5dc56-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5dc56-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5dc56-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5dc56-116">Not supported.</span></span>|
|<span data-ttu-id="5dc56-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5dc56-117">Application</span></span>|<span data-ttu-id="5dc56-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5dc56-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5dc56-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5dc56-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="5dc56-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5dc56-120">Request headers</span></span>
|<span data-ttu-id="5dc56-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5dc56-121">Header</span></span>|<span data-ttu-id="5dc56-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5dc56-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5dc56-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5dc56-123">Authorization</span></span>|<span data-ttu-id="5dc56-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5dc56-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5dc56-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5dc56-125">Accept</span></span>|<span data-ttu-id="5dc56-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5dc56-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5dc56-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5dc56-127">Request body</span></span>
<span data-ttu-id="5dc56-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionAppLockerFile.</span><span class="sxs-lookup"><span data-stu-id="5dc56-128">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="5dc56-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionAppLockerFile.</span><span class="sxs-lookup"><span data-stu-id="5dc56-129">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="5dc56-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5dc56-130">Property</span></span>|<span data-ttu-id="5dc56-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5dc56-131">Type</span></span>|<span data-ttu-id="5dc56-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5dc56-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5dc56-133">displayName</span><span class="sxs-lookup"><span data-stu-id="5dc56-133">displayName</span></span>|<span data-ttu-id="5dc56-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5dc56-134">String</span></span>|<span data-ttu-id="5dc56-135">O nome amigável</span><span class="sxs-lookup"><span data-stu-id="5dc56-135">The friendly name</span></span>|
|<span data-ttu-id="5dc56-136">fileHash</span><span class="sxs-lookup"><span data-stu-id="5dc56-136">fileHash</span></span>|<span data-ttu-id="5dc56-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5dc56-137">String</span></span>|<span data-ttu-id="5dc56-138">Hash SHA256 do arquivo</span><span class="sxs-lookup"><span data-stu-id="5dc56-138">SHA256 hash of the file</span></span>|
|<span data-ttu-id="5dc56-139">file</span><span class="sxs-lookup"><span data-stu-id="5dc56-139">file</span></span>|<span data-ttu-id="5dc56-140">Binária</span><span class="sxs-lookup"><span data-stu-id="5dc56-140">Binary</span></span>|<span data-ttu-id="5dc56-141">Arquivo como uma matriz de bytes</span><span class="sxs-lookup"><span data-stu-id="5dc56-141">File as a byte array</span></span>|
|<span data-ttu-id="5dc56-142">id</span><span class="sxs-lookup"><span data-stu-id="5dc56-142">id</span></span>|<span data-ttu-id="5dc56-143">String</span><span class="sxs-lookup"><span data-stu-id="5dc56-143">String</span></span>|<span data-ttu-id="5dc56-144">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5dc56-144">Key of the entity.</span></span>|
|<span data-ttu-id="5dc56-145">version</span><span class="sxs-lookup"><span data-stu-id="5dc56-145">version</span></span>|<span data-ttu-id="5dc56-146">String</span><span class="sxs-lookup"><span data-stu-id="5dc56-146">String</span></span>|<span data-ttu-id="5dc56-147">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="5dc56-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="5dc56-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dc56-148">Response</span></span>
<span data-ttu-id="5dc56-149">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5dc56-149">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5dc56-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5dc56-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="5dc56-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5dc56-151">Request</span></span>
<span data-ttu-id="5dc56-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5dc56-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5dc56-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dc56-153">Response</span></span>
<span data-ttu-id="5dc56-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5dc56-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




