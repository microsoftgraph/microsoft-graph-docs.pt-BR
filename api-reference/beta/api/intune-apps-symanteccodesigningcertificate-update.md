---
title: Atualizar symantecCodeSigningCertificate
description: Atualiza as propriedades de um objeto symantecCodeSigningCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 27d4833c82819c5a646cbad25959bdb6071a782c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450626"
---
# <a name="update-symanteccodesigningcertificate"></a><span data-ttu-id="6bb03-103">Atualizar symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="6bb03-103">Update symantecCodeSigningCertificate</span></span>

<span data-ttu-id="6bb03-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6bb03-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6bb03-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6bb03-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6bb03-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6bb03-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6bb03-107">Atualiza as propriedades de um objeto [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="6bb03-107">Update the properties of a [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6bb03-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6bb03-108">Prerequisites</span></span>
<span data-ttu-id="6bb03-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bb03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bb03-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6bb03-111">Permission type</span></span>|<span data-ttu-id="6bb03-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6bb03-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6bb03-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6bb03-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6bb03-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bb03-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6bb03-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6bb03-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6bb03-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6bb03-116">Not supported.</span></span>|
|<span data-ttu-id="6bb03-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6bb03-117">Application</span></span>|<span data-ttu-id="6bb03-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bb03-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6bb03-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6bb03-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/symantecCodeSigningCertificate
```

## <a name="request-headers"></a><span data-ttu-id="6bb03-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6bb03-120">Request headers</span></span>
|<span data-ttu-id="6bb03-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6bb03-121">Header</span></span>|<span data-ttu-id="6bb03-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6bb03-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6bb03-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6bb03-123">Authorization</span></span>|<span data-ttu-id="6bb03-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6bb03-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6bb03-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6bb03-125">Accept</span></span>|<span data-ttu-id="6bb03-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6bb03-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bb03-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6bb03-127">Request body</span></span>
<span data-ttu-id="6bb03-128">No corpo da solicitação, forneça uma representação JSON do objeto [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="6bb03-128">In the request body, supply a JSON representation for the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

<span data-ttu-id="6bb03-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="6bb03-129">The following table shows the properties that are required when you create the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md).</span></span>

|<span data-ttu-id="6bb03-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6bb03-130">Property</span></span>|<span data-ttu-id="6bb03-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6bb03-131">Type</span></span>|<span data-ttu-id="6bb03-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bb03-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bb03-133">id</span><span class="sxs-lookup"><span data-stu-id="6bb03-133">id</span></span>|<span data-ttu-id="6bb03-134">String</span><span class="sxs-lookup"><span data-stu-id="6bb03-134">String</span></span>|<span data-ttu-id="6bb03-135">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6bb03-135">The key of the entity.</span></span>|
|<span data-ttu-id="6bb03-136">conteúdo</span><span class="sxs-lookup"><span data-stu-id="6bb03-136">content</span></span>|<span data-ttu-id="6bb03-137">Binária</span><span class="sxs-lookup"><span data-stu-id="6bb03-137">Binary</span></span>|<span data-ttu-id="6bb03-138">O certificado de assinatura de código Symantec do Windows no formato de dados brutos.</span><span class="sxs-lookup"><span data-stu-id="6bb03-138">The Windows Symantec Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="6bb03-139">status</span><span class="sxs-lookup"><span data-stu-id="6bb03-139">status</span></span>|[<span data-ttu-id="6bb03-140">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="6bb03-140">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="6bb03-141">O status do certificado provisionado ou não foi provisionado.</span><span class="sxs-lookup"><span data-stu-id="6bb03-141">The Cert Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="6bb03-142">Os valores possíveis são: `notProvisioned` e `provisioned`.</span><span class="sxs-lookup"><span data-stu-id="6bb03-142">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="6bb03-143">password</span><span class="sxs-lookup"><span data-stu-id="6bb03-143">password</span></span>|<span data-ttu-id="6bb03-144">String</span><span class="sxs-lookup"><span data-stu-id="6bb03-144">String</span></span>|<span data-ttu-id="6bb03-145">A senha necessária para o arquivo. pfx.</span><span class="sxs-lookup"><span data-stu-id="6bb03-145">The Password required for .pfx file.</span></span>|
|<span data-ttu-id="6bb03-146">SubjectName</span><span class="sxs-lookup"><span data-stu-id="6bb03-146">subjectName</span></span>|<span data-ttu-id="6bb03-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6bb03-147">String</span></span>|<span data-ttu-id="6bb03-148">O nome da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="6bb03-148">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="6bb03-149">assunto</span><span class="sxs-lookup"><span data-stu-id="6bb03-149">subject</span></span>|<span data-ttu-id="6bb03-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6bb03-150">String</span></span>|<span data-ttu-id="6bb03-151">O valor de entidade para o certificado.</span><span class="sxs-lookup"><span data-stu-id="6bb03-151">The Subject value for the cert.</span></span>|
|<span data-ttu-id="6bb03-152">issuerName</span><span class="sxs-lookup"><span data-stu-id="6bb03-152">issuerName</span></span>|<span data-ttu-id="6bb03-153">String</span><span class="sxs-lookup"><span data-stu-id="6bb03-153">String</span></span>|<span data-ttu-id="6bb03-154">O nome do emissor do certificado.</span><span class="sxs-lookup"><span data-stu-id="6bb03-154">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="6bb03-155">emissor</span><span class="sxs-lookup"><span data-stu-id="6bb03-155">issuer</span></span>|<span data-ttu-id="6bb03-156">String</span><span class="sxs-lookup"><span data-stu-id="6bb03-156">String</span></span>|<span data-ttu-id="6bb03-157">O valor do emissor para o certificado.</span><span class="sxs-lookup"><span data-stu-id="6bb03-157">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="6bb03-158">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6bb03-158">expirationDateTime</span></span>|<span data-ttu-id="6bb03-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bb03-159">DateTimeOffset</span></span>|<span data-ttu-id="6bb03-160">A data de expiração do certificado.</span><span class="sxs-lookup"><span data-stu-id="6bb03-160">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="6bb03-161">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="6bb03-161">uploadDateTime</span></span>|<span data-ttu-id="6bb03-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bb03-162">DateTimeOffset</span></span>|<span data-ttu-id="6bb03-163">O tipo do certificado de codesignação como CERT da Symantec.</span><span class="sxs-lookup"><span data-stu-id="6bb03-163">The Type of the CodeSigning Cert as Symantec Cert.</span></span>|



## <a name="response"></a><span data-ttu-id="6bb03-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bb03-164">Response</span></span>
<span data-ttu-id="6bb03-165">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6bb03-165">If successful, this method returns a `200 OK` response code and an updated [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6bb03-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6bb03-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="6bb03-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6bb03-167">Request</span></span>
<span data-ttu-id="6bb03-168">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6bb03-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/symantecCodeSigningCertificate
Content-type: application/json
Content-length: 421

{
  "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
  "content": "Y29udGVudA==",
  "status": "provisioned",
  "password": "Password value",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00"
}
```

### <a name="response"></a><span data-ttu-id="6bb03-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bb03-169">Response</span></span>
<span data-ttu-id="6bb03-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6bb03-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 470

{
  "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
  "id": "00ffe83e-e83e-00ff-3ee8-ff003ee8ff00",
  "content": "Y29udGVudA==",
  "status": "provisioned",
  "password": "Password value",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00"
}
```





