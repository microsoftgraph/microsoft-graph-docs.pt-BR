---
title: Atualizar symantecCodeSigningCertificate
description: Atualiza as propriedades de um objeto symantecCodeSigningCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d21f72c62bd31bb25312e2b86835c339807d81ae
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32488775"
---
# <a name="update-symanteccodesigningcertificate"></a><span data-ttu-id="4c435-103">Atualizar symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="4c435-103">Update symantecCodeSigningCertificate</span></span>

> <span data-ttu-id="4c435-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4c435-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c435-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4c435-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c435-106">Atualiza as propriedades de um objeto [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="4c435-106">Update the properties of a [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c435-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4c435-107">Prerequisites</span></span>
<span data-ttu-id="4c435-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c435-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c435-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c435-110">Permission type</span></span>|<span data-ttu-id="4c435-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4c435-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c435-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c435-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4c435-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c435-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4c435-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c435-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c435-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c435-115">Not supported.</span></span>|
|<span data-ttu-id="4c435-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c435-116">Application</span></span>|<span data-ttu-id="4c435-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c435-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c435-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c435-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/symantecCodeSigningCertificate
```

## <a name="request-headers"></a><span data-ttu-id="4c435-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c435-119">Request headers</span></span>
|<span data-ttu-id="4c435-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4c435-120">Header</span></span>|<span data-ttu-id="4c435-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4c435-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c435-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c435-122">Authorization</span></span>|<span data-ttu-id="4c435-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c435-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c435-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4c435-124">Accept</span></span>|<span data-ttu-id="4c435-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4c435-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c435-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c435-126">Request body</span></span>
<span data-ttu-id="4c435-127">No corpo da solicitação, forneça uma representação JSON do objeto [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="4c435-127">In the request body, supply a JSON representation for the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

<span data-ttu-id="4c435-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="4c435-128">The following table shows the properties that are required when you create the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md).</span></span>

|<span data-ttu-id="4c435-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4c435-129">Property</span></span>|<span data-ttu-id="4c435-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c435-130">Type</span></span>|<span data-ttu-id="4c435-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c435-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c435-132">id</span><span class="sxs-lookup"><span data-stu-id="4c435-132">id</span></span>|<span data-ttu-id="4c435-133">String</span><span class="sxs-lookup"><span data-stu-id="4c435-133">String</span></span>|<span data-ttu-id="4c435-134">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4c435-134">The key of the entity.</span></span>|
|<span data-ttu-id="4c435-135">conteúdo</span><span class="sxs-lookup"><span data-stu-id="4c435-135">content</span></span>|<span data-ttu-id="4c435-136">Binary</span><span class="sxs-lookup"><span data-stu-id="4c435-136">Binary</span></span>|<span data-ttu-id="4c435-137">O certificado de assinatura de código Symantec do Windows no formato de dados brutos.</span><span class="sxs-lookup"><span data-stu-id="4c435-137">The Windows Symantec Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="4c435-138">status</span><span class="sxs-lookup"><span data-stu-id="4c435-138">status</span></span>|[<span data-ttu-id="4c435-139">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="4c435-139">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="4c435-140">O status do certificado provisionado ou não foi provisionado.</span><span class="sxs-lookup"><span data-stu-id="4c435-140">The Cert Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="4c435-141">Os valores possíveis são: `notProvisioned` e `provisioned`.</span><span class="sxs-lookup"><span data-stu-id="4c435-141">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="4c435-142">password</span><span class="sxs-lookup"><span data-stu-id="4c435-142">password</span></span>|<span data-ttu-id="4c435-143">String</span><span class="sxs-lookup"><span data-stu-id="4c435-143">String</span></span>|<span data-ttu-id="4c435-144">A senha necessária para o arquivo. pfx.</span><span class="sxs-lookup"><span data-stu-id="4c435-144">The Password required for .pfx file.</span></span>|
|<span data-ttu-id="4c435-145">SubjectName</span><span class="sxs-lookup"><span data-stu-id="4c435-145">subjectName</span></span>|<span data-ttu-id="4c435-146">String</span><span class="sxs-lookup"><span data-stu-id="4c435-146">String</span></span>|<span data-ttu-id="4c435-147">O nome da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="4c435-147">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="4c435-148">Assunto</span><span class="sxs-lookup"><span data-stu-id="4c435-148">subject</span></span>|<span data-ttu-id="4c435-149">String</span><span class="sxs-lookup"><span data-stu-id="4c435-149">String</span></span>|<span data-ttu-id="4c435-150">O valor de entidade para o certificado.</span><span class="sxs-lookup"><span data-stu-id="4c435-150">The Subject value for the cert.</span></span>|
|<span data-ttu-id="4c435-151">issuerName</span><span class="sxs-lookup"><span data-stu-id="4c435-151">issuerName</span></span>|<span data-ttu-id="4c435-152">String</span><span class="sxs-lookup"><span data-stu-id="4c435-152">String</span></span>|<span data-ttu-id="4c435-153">O nome do emissor do certificado.</span><span class="sxs-lookup"><span data-stu-id="4c435-153">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="4c435-154">emissor</span><span class="sxs-lookup"><span data-stu-id="4c435-154">issuer</span></span>|<span data-ttu-id="4c435-155">String</span><span class="sxs-lookup"><span data-stu-id="4c435-155">String</span></span>|<span data-ttu-id="4c435-156">O valor do emissor para o certificado.</span><span class="sxs-lookup"><span data-stu-id="4c435-156">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="4c435-157">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4c435-157">expirationDateTime</span></span>|<span data-ttu-id="4c435-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c435-158">DateTimeOffset</span></span>|<span data-ttu-id="4c435-159">A data de expiração do certificado.</span><span class="sxs-lookup"><span data-stu-id="4c435-159">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="4c435-160">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="4c435-160">uploadDateTime</span></span>|<span data-ttu-id="4c435-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c435-161">DateTimeOffset</span></span>|<span data-ttu-id="4c435-162">O tipo do certificado de codeSignação como CERT da Symantec.</span><span class="sxs-lookup"><span data-stu-id="4c435-162">The Type of the CodeSigning Cert as Symantec Cert.</span></span>|



## <a name="response"></a><span data-ttu-id="4c435-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c435-163">Response</span></span>
<span data-ttu-id="4c435-164">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c435-164">If successful, this method returns a `200 OK` response code and an updated [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c435-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c435-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c435-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c435-166">Request</span></span>
<span data-ttu-id="4c435-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c435-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4c435-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c435-168">Response</span></span>
<span data-ttu-id="4c435-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4c435-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





