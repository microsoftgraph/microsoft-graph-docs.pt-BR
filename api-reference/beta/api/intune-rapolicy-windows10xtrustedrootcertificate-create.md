---
title: Criar windows10XTrustedRootCertificate
description: Criar um novo objeto windows10XTrustedRootCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7b8a8995988a0eedd2f8204db12c9eb4ded184d3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241299"
---
# <a name="create-windows10xtrustedrootcertificate"></a><span data-ttu-id="7ac3e-103">Criar windows10XTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="7ac3e-103">Create windows10XTrustedRootCertificate</span></span>

<span data-ttu-id="7ac3e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ac3e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ac3e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7ac3e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ac3e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7ac3e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ac3e-107">Criar um novo objeto [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="7ac3e-107">Create a new [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ac3e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7ac3e-108">Prerequisites</span></span>
<span data-ttu-id="7ac3e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ac3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ac3e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ac3e-111">Permission type</span></span>|<span data-ttu-id="7ac3e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7ac3e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ac3e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ac3e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7ac3e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ac3e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7ac3e-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ac3e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ac3e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ac3e-116">Not supported.</span></span>|
|<span data-ttu-id="7ac3e-117">Application</span><span class="sxs-lookup"><span data-stu-id="7ac3e-117">Application</span></span>|<span data-ttu-id="7ac3e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ac3e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ac3e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ac3e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceAccessProfiles
```

## <a name="request-headers"></a><span data-ttu-id="7ac3e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ac3e-120">Request headers</span></span>
|<span data-ttu-id="7ac3e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7ac3e-121">Header</span></span>|<span data-ttu-id="7ac3e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7ac3e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ac3e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ac3e-123">Authorization</span></span>|<span data-ttu-id="7ac3e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ac3e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ac3e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7ac3e-125">Accept</span></span>|<span data-ttu-id="7ac3e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7ac3e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ac3e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ac3e-127">Request body</span></span>
<span data-ttu-id="7ac3e-128">No corpo da solicitação, forneça uma representação JSON do objeto windows10XTrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="7ac3e-128">In the request body, supply a JSON representation for the windows10XTrustedRootCertificate object.</span></span>

<span data-ttu-id="7ac3e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10XTrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="7ac3e-129">The following table shows the properties that are required when you create the windows10XTrustedRootCertificate.</span></span>

|<span data-ttu-id="7ac3e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ac3e-130">Property</span></span>|<span data-ttu-id="7ac3e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ac3e-131">Type</span></span>|<span data-ttu-id="7ac3e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ac3e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ac3e-133">id</span><span class="sxs-lookup"><span data-stu-id="7ac3e-133">id</span></span>|<span data-ttu-id="7ac3e-134">String</span><span class="sxs-lookup"><span data-stu-id="7ac3e-134">String</span></span>|<span data-ttu-id="7ac3e-135">Identificador de perfil herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7ac3e-135">Profile identifier Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="7ac3e-136">versão</span><span class="sxs-lookup"><span data-stu-id="7ac3e-136">version</span></span>|<span data-ttu-id="7ac3e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="7ac3e-137">Int32</span></span>|<span data-ttu-id="7ac3e-138">Versão do perfil herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7ac3e-138">Version of the profile Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="7ac3e-139">displayName</span><span class="sxs-lookup"><span data-stu-id="7ac3e-139">displayName</span></span>|<span data-ttu-id="7ac3e-140">String</span><span class="sxs-lookup"><span data-stu-id="7ac3e-140">String</span></span>|<span data-ttu-id="7ac3e-141">Nome de exibição do perfil herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7ac3e-141">Profile display name Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="7ac3e-142">description</span><span class="sxs-lookup"><span data-stu-id="7ac3e-142">description</span></span>|<span data-ttu-id="7ac3e-143">String</span><span class="sxs-lookup"><span data-stu-id="7ac3e-143">String</span></span>|<span data-ttu-id="7ac3e-144">Descrição do perfil herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7ac3e-144">Profile description Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="7ac3e-145">creationDatetime</span><span class="sxs-lookup"><span data-stu-id="7ac3e-145">creationDateTime</span></span>|<span data-ttu-id="7ac3e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ac3e-146">DateTimeOffset</span></span>|<span data-ttu-id="7ac3e-147">O perfil DateTime foi criado herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7ac3e-147">DateTime profile was created Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="7ac3e-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7ac3e-148">lastModifiedDateTime</span></span>|<span data-ttu-id="7ac3e-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ac3e-149">DateTimeOffset</span></span>|<span data-ttu-id="7ac3e-150">O perfil DateTime foi modificado pela última vez de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7ac3e-150">DateTime profile was last modified Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="7ac3e-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7ac3e-151">roleScopeTagIds</span></span>|<span data-ttu-id="7ac3e-152">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ac3e-152">String collection</span></span>|<span data-ttu-id="7ac3e-153">Marcas de escopo herdadas de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7ac3e-153">Scope Tags Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="7ac3e-154">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="7ac3e-154">trustedRootCertificate</span></span>|<span data-ttu-id="7ac3e-155">Binária</span><span class="sxs-lookup"><span data-stu-id="7ac3e-155">Binary</span></span>|<span data-ttu-id="7ac3e-156">Certificado raiz confiável</span><span class="sxs-lookup"><span data-stu-id="7ac3e-156">Trusted Root Certificate</span></span>|
|<span data-ttu-id="7ac3e-157">certFileName</span><span class="sxs-lookup"><span data-stu-id="7ac3e-157">certFileName</span></span>|<span data-ttu-id="7ac3e-158">String</span><span class="sxs-lookup"><span data-stu-id="7ac3e-158">String</span></span>|<span data-ttu-id="7ac3e-159">Nome do arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="7ac3e-159">File name to display in UI.</span></span>|
|<span data-ttu-id="7ac3e-160">destinationStore</span><span class="sxs-lookup"><span data-stu-id="7ac3e-160">destinationStore</span></span>|[<span data-ttu-id="7ac3e-161">certificateDestinationStore</span><span class="sxs-lookup"><span data-stu-id="7ac3e-161">certificateDestinationStore</span></span>](../resources/intune-shared-certificatedestinationstore.md)|<span data-ttu-id="7ac3e-162">Local do repositório de destino para o certificado raiz confiável.</span><span class="sxs-lookup"><span data-stu-id="7ac3e-162">Destination store location for the Trusted Root Certificate.</span></span> <span data-ttu-id="7ac3e-163">Os valores possíveis são: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span><span class="sxs-lookup"><span data-stu-id="7ac3e-163">Possible values are: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span></span>|



## <a name="response"></a><span data-ttu-id="7ac3e-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ac3e-164">Response</span></span>
<span data-ttu-id="7ac3e-165">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ac3e-165">If successful, this method returns a `201 Created` response code and a [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ac3e-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7ac3e-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ac3e-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ac3e-167">Request</span></span>
<span data-ttu-id="7ac3e-168">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ac3e-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles
Content-type: application/json
Content-length: 456

{
  "@odata.type": "#microsoft.graph.windows10XTrustedRootCertificate",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value",
  "destinationStore": "computerCertStoreIntermediate"
}
```

### <a name="response"></a><span data-ttu-id="7ac3e-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ac3e-169">Response</span></span>
<span data-ttu-id="7ac3e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7ac3e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 569

{
  "@odata.type": "#microsoft.graph.windows10XTrustedRootCertificate",
  "id": "be0bfd01-fd01-be0b-01fd-0bbe01fd0bbe",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value",
  "destinationStore": "computerCertStoreIntermediate"
}
```




