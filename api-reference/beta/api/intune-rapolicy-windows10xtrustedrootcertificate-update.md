---
title: Atualizar windows10XTrustedRootCertificate
description: Atualize as propriedades de um objeto windows10XTrustedRootCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0c8ba77096df428f7c5c99429c2b6bdeebac3e26
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145065"
---
# <a name="update-windows10xtrustedrootcertificate"></a><span data-ttu-id="7f8a7-103">Atualizar windows10XTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="7f8a7-103">Update windows10XTrustedRootCertificate</span></span>

<span data-ttu-id="7f8a7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f8a7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f8a7-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7f8a7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f8a7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7f8a7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f8a7-107">Atualize as propriedades de um [objeto windows10XTrustedRootCertificate.](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="7f8a7-107">Update the properties of a [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f8a7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7f8a7-108">Prerequisites</span></span>
<span data-ttu-id="7f8a7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f8a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f8a7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f8a7-111">Permission type</span></span>|<span data-ttu-id="7f8a7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7f8a7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f8a7-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f8a7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7f8a7-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f8a7-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7f8a7-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f8a7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f8a7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f8a7-116">Not supported.</span></span>|
|<span data-ttu-id="7f8a7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f8a7-117">Application</span></span>|<span data-ttu-id="7f8a7-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f8a7-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f8a7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f8a7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}
```

## <a name="request-headers"></a><span data-ttu-id="7f8a7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f8a7-120">Request headers</span></span>
|<span data-ttu-id="7f8a7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7f8a7-121">Header</span></span>|<span data-ttu-id="7f8a7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7f8a7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f8a7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f8a7-123">Authorization</span></span>|<span data-ttu-id="7f8a7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f8a7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f8a7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7f8a7-125">Accept</span></span>|<span data-ttu-id="7f8a7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7f8a7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f8a7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f8a7-127">Request body</span></span>
<span data-ttu-id="7f8a7-128">No corpo da solicitação, fornece uma representação JSON para o [objeto windows10XTrustedRootCertificate.](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="7f8a7-128">In the request body, supply a JSON representation for the [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="7f8a7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="7f8a7-129">The following table shows the properties that are required when you create the [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md).</span></span>

|<span data-ttu-id="7f8a7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f8a7-130">Property</span></span>|<span data-ttu-id="7f8a7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f8a7-131">Type</span></span>|<span data-ttu-id="7f8a7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f8a7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f8a7-133">id</span><span class="sxs-lookup"><span data-stu-id="7f8a7-133">id</span></span>|<span data-ttu-id="7f8a7-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f8a7-134">String</span></span>|<span data-ttu-id="7f8a7-135">Identificador de perfil Herdado [de deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7f8a7-135">Profile identifier Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="7f8a7-136">versão</span><span class="sxs-lookup"><span data-stu-id="7f8a7-136">version</span></span>|<span data-ttu-id="7f8a7-137">Int32</span><span class="sxs-lookup"><span data-stu-id="7f8a7-137">Int32</span></span>|<span data-ttu-id="7f8a7-138">Versão do perfil Herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7f8a7-138">Version of the profile Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="7f8a7-139">displayName</span><span class="sxs-lookup"><span data-stu-id="7f8a7-139">displayName</span></span>|<span data-ttu-id="7f8a7-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f8a7-140">String</span></span>|<span data-ttu-id="7f8a7-141">Nome de exibição de perfil Herdado [de deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7f8a7-141">Profile display name Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="7f8a7-142">descrição</span><span class="sxs-lookup"><span data-stu-id="7f8a7-142">description</span></span>|<span data-ttu-id="7f8a7-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f8a7-143">String</span></span>|<span data-ttu-id="7f8a7-144">Descrição de perfil [Herdada de deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7f8a7-144">Profile description Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="7f8a7-145">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="7f8a7-145">creationDateTime</span></span>|<span data-ttu-id="7f8a7-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f8a7-146">DateTimeOffset</span></span>|<span data-ttu-id="7f8a7-147">Perfil DateTime foi criado Herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7f8a7-147">DateTime profile was created Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="7f8a7-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f8a7-148">lastModifiedDateTime</span></span>|<span data-ttu-id="7f8a7-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f8a7-149">DateTimeOffset</span></span>|<span data-ttu-id="7f8a7-150">O perfil DateTime foi modificado pela última vez Herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7f8a7-150">DateTime profile was last modified Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="7f8a7-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7f8a7-151">roleScopeTagIds</span></span>|<span data-ttu-id="7f8a7-152">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f8a7-152">String collection</span></span>|<span data-ttu-id="7f8a7-153">Marcas de escopo herdadas [de deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7f8a7-153">Scope Tags Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="7f8a7-154">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="7f8a7-154">trustedRootCertificate</span></span>|<span data-ttu-id="7f8a7-155">Binário</span><span class="sxs-lookup"><span data-stu-id="7f8a7-155">Binary</span></span>|<span data-ttu-id="7f8a7-156">Certificado Raiz Confiável</span><span class="sxs-lookup"><span data-stu-id="7f8a7-156">Trusted Root Certificate</span></span>|
|<span data-ttu-id="7f8a7-157">certFileName</span><span class="sxs-lookup"><span data-stu-id="7f8a7-157">certFileName</span></span>|<span data-ttu-id="7f8a7-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f8a7-158">String</span></span>|<span data-ttu-id="7f8a7-159">Nome do arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="7f8a7-159">File name to display in UI.</span></span>|
|<span data-ttu-id="7f8a7-160">destinationStore</span><span class="sxs-lookup"><span data-stu-id="7f8a7-160">destinationStore</span></span>|[<span data-ttu-id="7f8a7-161">certificateDestinationStore</span><span class="sxs-lookup"><span data-stu-id="7f8a7-161">certificateDestinationStore</span></span>](../resources/intune-shared-certificatedestinationstore.md)|<span data-ttu-id="7f8a7-162">Local do armazenamento de destino para o Certificado Raiz Confiável.</span><span class="sxs-lookup"><span data-stu-id="7f8a7-162">Destination store location for the Trusted Root Certificate.</span></span> <span data-ttu-id="7f8a7-163">Os valores possíveis são: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span><span class="sxs-lookup"><span data-stu-id="7f8a7-163">Possible values are: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span></span>|



## <a name="response"></a><span data-ttu-id="7f8a7-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f8a7-164">Response</span></span>
<span data-ttu-id="7f8a7-165">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f8a7-165">If successful, this method returns a `200 OK` response code and an updated [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f8a7-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f8a7-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f8a7-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f8a7-167">Request</span></span>
<span data-ttu-id="7f8a7-168">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f8a7-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}
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

### <a name="response"></a><span data-ttu-id="7f8a7-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f8a7-169">Response</span></span>
<span data-ttu-id="7f8a7-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7f8a7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




