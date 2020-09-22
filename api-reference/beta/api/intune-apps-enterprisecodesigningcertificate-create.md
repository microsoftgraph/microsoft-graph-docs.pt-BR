---
title: Criar enterpriseCodeSigningCertificate
description: Criar um novo objeto enterpriseCodeSigningCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ad49562a3e9c667f0ccec6dc91f67222a164e09f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48001173"
---
# <a name="create-enterprisecodesigningcertificate"></a><span data-ttu-id="18d79-103">Criar enterpriseCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="18d79-103">Create enterpriseCodeSigningCertificate</span></span>

<span data-ttu-id="18d79-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18d79-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18d79-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="18d79-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18d79-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="18d79-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18d79-107">Criar um novo objeto [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="18d79-107">Create a new [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18d79-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="18d79-108">Prerequisites</span></span>
<span data-ttu-id="18d79-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18d79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18d79-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18d79-111">Permission type</span></span>|<span data-ttu-id="18d79-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="18d79-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18d79-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18d79-113">Delegated (work or school account)</span></span>|<span data-ttu-id="18d79-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18d79-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="18d79-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18d79-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18d79-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18d79-116">Not supported.</span></span>|
|<span data-ttu-id="18d79-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18d79-117">Application</span></span>|<span data-ttu-id="18d79-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18d79-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="18d79-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18d79-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/enterpriseCodeSigningCertificates
```

## <a name="request-headers"></a><span data-ttu-id="18d79-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18d79-120">Request headers</span></span>
|<span data-ttu-id="18d79-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="18d79-121">Header</span></span>|<span data-ttu-id="18d79-122">Valor</span><span class="sxs-lookup"><span data-stu-id="18d79-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18d79-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="18d79-123">Authorization</span></span>|<span data-ttu-id="18d79-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18d79-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18d79-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="18d79-125">Accept</span></span>|<span data-ttu-id="18d79-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18d79-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18d79-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18d79-127">Request body</span></span>
<span data-ttu-id="18d79-128">No corpo da solicitação, forneça uma representação JSON do objeto enterpriseCodeSigningCertificate.</span><span class="sxs-lookup"><span data-stu-id="18d79-128">In the request body, supply a JSON representation for the enterpriseCodeSigningCertificate object.</span></span>

<span data-ttu-id="18d79-129">A tabela a seguir mostra as propriedades que são necessárias ao criar enterpriseCodeSigningCertificate.</span><span class="sxs-lookup"><span data-stu-id="18d79-129">The following table shows the properties that are required when you create the enterpriseCodeSigningCertificate.</span></span>

|<span data-ttu-id="18d79-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18d79-130">Property</span></span>|<span data-ttu-id="18d79-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="18d79-131">Type</span></span>|<span data-ttu-id="18d79-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="18d79-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18d79-133">id</span><span class="sxs-lookup"><span data-stu-id="18d79-133">id</span></span>|<span data-ttu-id="18d79-134">String</span><span class="sxs-lookup"><span data-stu-id="18d79-134">String</span></span>|<span data-ttu-id="18d79-135">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="18d79-135">The key of the entity.</span></span>|
|<span data-ttu-id="18d79-136">conteúdo</span><span class="sxs-lookup"><span data-stu-id="18d79-136">content</span></span>|<span data-ttu-id="18d79-137">Binária</span><span class="sxs-lookup"><span data-stu-id="18d79-137">Binary</span></span>|<span data-ttu-id="18d79-138">O certificado de assinatura de código do Windows Enterprise no formato de dados brutos.</span><span class="sxs-lookup"><span data-stu-id="18d79-138">The Windows Enterprise Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="18d79-139">status</span><span class="sxs-lookup"><span data-stu-id="18d79-139">status</span></span>|[<span data-ttu-id="18d79-140">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="18d79-140">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="18d79-141">O status do certificado provisionado ou não foi provisionado.</span><span class="sxs-lookup"><span data-stu-id="18d79-141">The Certificate Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="18d79-142">Os valores possíveis são: `notProvisioned` e `provisioned`.</span><span class="sxs-lookup"><span data-stu-id="18d79-142">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="18d79-143">SubjectName</span><span class="sxs-lookup"><span data-stu-id="18d79-143">subjectName</span></span>|<span data-ttu-id="18d79-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18d79-144">String</span></span>|<span data-ttu-id="18d79-145">O nome da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="18d79-145">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="18d79-146">assunto</span><span class="sxs-lookup"><span data-stu-id="18d79-146">subject</span></span>|<span data-ttu-id="18d79-147">String</span><span class="sxs-lookup"><span data-stu-id="18d79-147">String</span></span>|<span data-ttu-id="18d79-148">O valor de entidade para o certificado.</span><span class="sxs-lookup"><span data-stu-id="18d79-148">The Subject Value for the cert.</span></span>|
|<span data-ttu-id="18d79-149">issuerName</span><span class="sxs-lookup"><span data-stu-id="18d79-149">issuerName</span></span>|<span data-ttu-id="18d79-150">String</span><span class="sxs-lookup"><span data-stu-id="18d79-150">String</span></span>|<span data-ttu-id="18d79-151">O nome do emissor do certificado.</span><span class="sxs-lookup"><span data-stu-id="18d79-151">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="18d79-152">emissor</span><span class="sxs-lookup"><span data-stu-id="18d79-152">issuer</span></span>|<span data-ttu-id="18d79-153">String</span><span class="sxs-lookup"><span data-stu-id="18d79-153">String</span></span>|<span data-ttu-id="18d79-154">O valor do emissor para o certificado.</span><span class="sxs-lookup"><span data-stu-id="18d79-154">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="18d79-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="18d79-155">expirationDateTime</span></span>|<span data-ttu-id="18d79-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18d79-156">DateTimeOffset</span></span>|<span data-ttu-id="18d79-157">A data de expiração do certificado.</span><span class="sxs-lookup"><span data-stu-id="18d79-157">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="18d79-158">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="18d79-158">uploadDateTime</span></span>|<span data-ttu-id="18d79-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18d79-159">DateTimeOffset</span></span>|<span data-ttu-id="18d79-160">A data/hora do certificado de codesignação quando é carregado.</span><span class="sxs-lookup"><span data-stu-id="18d79-160">The date time of CodeSigning Cert when it is uploaded.</span></span>|



## <a name="response"></a><span data-ttu-id="18d79-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="18d79-161">Response</span></span>
<span data-ttu-id="18d79-162">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18d79-162">If successful, this method returns a `201 Created` response code and a [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18d79-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="18d79-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="18d79-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18d79-164">Request</span></span>
<span data-ttu-id="18d79-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="18d79-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/enterpriseCodeSigningCertificates
Content-type: application/json
Content-length: 390

{
  "@odata.type": "#microsoft.graph.enterpriseCodeSigningCertificate",
  "content": "Y29udGVudA==",
  "status": "provisioned",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00"
}
```

### <a name="response"></a><span data-ttu-id="18d79-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="18d79-166">Response</span></span>
<span data-ttu-id="18d79-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="18d79-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 439

{
  "@odata.type": "#microsoft.graph.enterpriseCodeSigningCertificate",
  "id": "b20d3703-3703-b20d-0337-0db203370db2",
  "content": "Y29udGVudA==",
  "status": "provisioned",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00"
}
```






