---
title: Atualizar enterpriseCodeSigningCertificate
description: Atualiza as propriedades de um objeto enterpriseCodeSigningCertificate.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ccae1a99fae750808f8703bc8163738d4cf3ab84
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42762123"
---
# <a name="update-enterprisecodesigningcertificate"></a><span data-ttu-id="0529b-103">Atualizar enterpriseCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="0529b-103">Update enterpriseCodeSigningCertificate</span></span>

> <span data-ttu-id="0529b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0529b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0529b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0529b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0529b-106">Atualiza as propriedades de um objeto [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="0529b-106">Update the properties of a [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0529b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0529b-107">Prerequisites</span></span>
<span data-ttu-id="0529b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0529b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0529b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0529b-110">Permission type</span></span>|<span data-ttu-id="0529b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0529b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0529b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0529b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0529b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0529b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0529b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0529b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0529b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0529b-115">Not supported.</span></span>|
|<span data-ttu-id="0529b-116">Application</span><span class="sxs-lookup"><span data-stu-id="0529b-116">Application</span></span>|<span data-ttu-id="0529b-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0529b-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0529b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0529b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="0529b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0529b-119">Request headers</span></span>
|<span data-ttu-id="0529b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0529b-120">Header</span></span>|<span data-ttu-id="0529b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0529b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0529b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0529b-122">Authorization</span></span>|<span data-ttu-id="0529b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0529b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0529b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0529b-124">Accept</span></span>|<span data-ttu-id="0529b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0529b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0529b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0529b-126">Request body</span></span>
<span data-ttu-id="0529b-127">No corpo da solicitação, forneça uma representação JSON do objeto [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="0529b-127">In the request body, supply a JSON representation for the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

<span data-ttu-id="0529b-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="0529b-128">The following table shows the properties that are required when you create the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md).</span></span>

|<span data-ttu-id="0529b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0529b-129">Property</span></span>|<span data-ttu-id="0529b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0529b-130">Type</span></span>|<span data-ttu-id="0529b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0529b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0529b-132">id</span><span class="sxs-lookup"><span data-stu-id="0529b-132">id</span></span>|<span data-ttu-id="0529b-133">String</span><span class="sxs-lookup"><span data-stu-id="0529b-133">String</span></span>|<span data-ttu-id="0529b-134">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0529b-134">The key of the entity.</span></span>|
|<span data-ttu-id="0529b-135">conteúdo</span><span class="sxs-lookup"><span data-stu-id="0529b-135">content</span></span>|<span data-ttu-id="0529b-136">Binária</span><span class="sxs-lookup"><span data-stu-id="0529b-136">Binary</span></span>|<span data-ttu-id="0529b-137">O certificado de assinatura de código do Windows Enterprise no formato de dados brutos.</span><span class="sxs-lookup"><span data-stu-id="0529b-137">The Windows Enterprise Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="0529b-138">status</span><span class="sxs-lookup"><span data-stu-id="0529b-138">status</span></span>|[<span data-ttu-id="0529b-139">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="0529b-139">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="0529b-140">O status do certificado provisionado ou não foi provisionado.</span><span class="sxs-lookup"><span data-stu-id="0529b-140">The Certificate Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="0529b-141">Os valores possíveis são: `notProvisioned` e `provisioned`.</span><span class="sxs-lookup"><span data-stu-id="0529b-141">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="0529b-142">SubjectName</span><span class="sxs-lookup"><span data-stu-id="0529b-142">subjectName</span></span>|<span data-ttu-id="0529b-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0529b-143">String</span></span>|<span data-ttu-id="0529b-144">O nome da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="0529b-144">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="0529b-145">assunto</span><span class="sxs-lookup"><span data-stu-id="0529b-145">subject</span></span>|<span data-ttu-id="0529b-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0529b-146">String</span></span>|<span data-ttu-id="0529b-147">O valor de entidade para o certificado.</span><span class="sxs-lookup"><span data-stu-id="0529b-147">The Subject Value for the cert.</span></span>|
|<span data-ttu-id="0529b-148">issuerName</span><span class="sxs-lookup"><span data-stu-id="0529b-148">issuerName</span></span>|<span data-ttu-id="0529b-149">String</span><span class="sxs-lookup"><span data-stu-id="0529b-149">String</span></span>|<span data-ttu-id="0529b-150">O nome do emissor do certificado.</span><span class="sxs-lookup"><span data-stu-id="0529b-150">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="0529b-151">emissor</span><span class="sxs-lookup"><span data-stu-id="0529b-151">issuer</span></span>|<span data-ttu-id="0529b-152">String</span><span class="sxs-lookup"><span data-stu-id="0529b-152">String</span></span>|<span data-ttu-id="0529b-153">O valor do emissor para o certificado.</span><span class="sxs-lookup"><span data-stu-id="0529b-153">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="0529b-154">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0529b-154">expirationDateTime</span></span>|<span data-ttu-id="0529b-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0529b-155">DateTimeOffset</span></span>|<span data-ttu-id="0529b-156">A data de expiração do certificado.</span><span class="sxs-lookup"><span data-stu-id="0529b-156">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="0529b-157">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="0529b-157">uploadDateTime</span></span>|<span data-ttu-id="0529b-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0529b-158">DateTimeOffset</span></span>|<span data-ttu-id="0529b-159">A data/hora do certificado de codesignação quando é carregado.</span><span class="sxs-lookup"><span data-stu-id="0529b-159">The date time of CodeSigning Cert when it is uploaded.</span></span>|



## <a name="response"></a><span data-ttu-id="0529b-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="0529b-160">Response</span></span>
<span data-ttu-id="0529b-161">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0529b-161">If successful, this method returns a `200 OK` response code and an updated [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0529b-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0529b-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="0529b-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0529b-163">Request</span></span>
<span data-ttu-id="0529b-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0529b-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
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

### <a name="response"></a><span data-ttu-id="0529b-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="0529b-165">Response</span></span>
<span data-ttu-id="0529b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0529b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




