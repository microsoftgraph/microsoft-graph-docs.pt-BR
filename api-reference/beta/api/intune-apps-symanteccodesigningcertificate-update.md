---
title: Atualizar symantecCodeSigningCertificate
description: Atualize as propriedades de um objeto symantecCodeSigningCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bc1edeade6d629fa2eecd1fb6bb7b29eb96a5619
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51139388"
---
# <a name="update-symanteccodesigningcertificate"></a><span data-ttu-id="63b7b-103">Atualizar symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="63b7b-103">Update symantecCodeSigningCertificate</span></span>

<span data-ttu-id="63b7b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63b7b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63b7b-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="63b7b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63b7b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="63b7b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63b7b-107">Atualize as propriedades de um [objeto symantecCodeSigningCertificate.](../resources/intune-apps-symanteccodesigningcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="63b7b-107">Update the properties of a [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63b7b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="63b7b-108">Prerequisites</span></span>
<span data-ttu-id="63b7b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63b7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63b7b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63b7b-111">Permission type</span></span>|<span data-ttu-id="63b7b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="63b7b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63b7b-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63b7b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="63b7b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63b7b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="63b7b-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63b7b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63b7b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63b7b-116">Not supported.</span></span>|
|<span data-ttu-id="63b7b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63b7b-117">Application</span></span>|<span data-ttu-id="63b7b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63b7b-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="63b7b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63b7b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/symantecCodeSigningCertificate
```

## <a name="request-headers"></a><span data-ttu-id="63b7b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63b7b-120">Request headers</span></span>
|<span data-ttu-id="63b7b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="63b7b-121">Header</span></span>|<span data-ttu-id="63b7b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="63b7b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63b7b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="63b7b-123">Authorization</span></span>|<span data-ttu-id="63b7b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63b7b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63b7b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="63b7b-125">Accept</span></span>|<span data-ttu-id="63b7b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="63b7b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63b7b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63b7b-127">Request body</span></span>
<span data-ttu-id="63b7b-128">No corpo da solicitação, fornece uma representação JSON para o [objeto symantecCodeSigningCertificate.](../resources/intune-apps-symanteccodesigningcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="63b7b-128">In the request body, supply a JSON representation for the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

<span data-ttu-id="63b7b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="63b7b-129">The following table shows the properties that are required when you create the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md).</span></span>

|<span data-ttu-id="63b7b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63b7b-130">Property</span></span>|<span data-ttu-id="63b7b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="63b7b-131">Type</span></span>|<span data-ttu-id="63b7b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="63b7b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63b7b-133">id</span><span class="sxs-lookup"><span data-stu-id="63b7b-133">id</span></span>|<span data-ttu-id="63b7b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="63b7b-134">String</span></span>|<span data-ttu-id="63b7b-135">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="63b7b-135">The key of the entity.</span></span>|
|<span data-ttu-id="63b7b-136">conteúdo</span><span class="sxs-lookup"><span data-stu-id="63b7b-136">content</span></span>|<span data-ttu-id="63b7b-137">Binário</span><span class="sxs-lookup"><span data-stu-id="63b7b-137">Binary</span></span>|<span data-ttu-id="63b7b-138">O Certificado do Windows Symantec Code-Signing no formato de dados brutos.</span><span class="sxs-lookup"><span data-stu-id="63b7b-138">The Windows Symantec Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="63b7b-139">status</span><span class="sxs-lookup"><span data-stu-id="63b7b-139">status</span></span>|[<span data-ttu-id="63b7b-140">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="63b7b-140">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="63b7b-141">O Status do Certificado Provisionado ou não Provisionado.</span><span class="sxs-lookup"><span data-stu-id="63b7b-141">The Cert Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="63b7b-142">Os valores possíveis são: `notProvisioned` e `provisioned`.</span><span class="sxs-lookup"><span data-stu-id="63b7b-142">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="63b7b-143">password</span><span class="sxs-lookup"><span data-stu-id="63b7b-143">password</span></span>|<span data-ttu-id="63b7b-144">String</span><span class="sxs-lookup"><span data-stu-id="63b7b-144">String</span></span>|<span data-ttu-id="63b7b-145">A senha necessária para o arquivo .pfx.</span><span class="sxs-lookup"><span data-stu-id="63b7b-145">The Password required for .pfx file.</span></span>|
|<span data-ttu-id="63b7b-146">SubjectName</span><span class="sxs-lookup"><span data-stu-id="63b7b-146">subjectName</span></span>|<span data-ttu-id="63b7b-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="63b7b-147">String</span></span>|<span data-ttu-id="63b7b-148">O Nome do Assunto do certificado.</span><span class="sxs-lookup"><span data-stu-id="63b7b-148">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="63b7b-149">assunto</span><span class="sxs-lookup"><span data-stu-id="63b7b-149">subject</span></span>|<span data-ttu-id="63b7b-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="63b7b-150">String</span></span>|<span data-ttu-id="63b7b-151">O valor Subject do certificado.</span><span class="sxs-lookup"><span data-stu-id="63b7b-151">The Subject value for the cert.</span></span>|
|<span data-ttu-id="63b7b-152">issuerName</span><span class="sxs-lookup"><span data-stu-id="63b7b-152">issuerName</span></span>|<span data-ttu-id="63b7b-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="63b7b-153">String</span></span>|<span data-ttu-id="63b7b-154">O Nome do Emissor do certificado.</span><span class="sxs-lookup"><span data-stu-id="63b7b-154">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="63b7b-155">emissor</span><span class="sxs-lookup"><span data-stu-id="63b7b-155">issuer</span></span>|<span data-ttu-id="63b7b-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="63b7b-156">String</span></span>|<span data-ttu-id="63b7b-157">O valor emissor do certificado.</span><span class="sxs-lookup"><span data-stu-id="63b7b-157">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="63b7b-158">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="63b7b-158">expirationDateTime</span></span>|<span data-ttu-id="63b7b-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63b7b-159">DateTimeOffset</span></span>|<span data-ttu-id="63b7b-160">A Data de Expiração do Certificado.</span><span class="sxs-lookup"><span data-stu-id="63b7b-160">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="63b7b-161">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="63b7b-161">uploadDateTime</span></span>|<span data-ttu-id="63b7b-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63b7b-162">DateTimeOffset</span></span>|<span data-ttu-id="63b7b-163">O Tipo do Certificado de Design de Código como Certificado Symantec.</span><span class="sxs-lookup"><span data-stu-id="63b7b-163">The Type of the CodeSigning Cert as Symantec Cert.</span></span>|



## <a name="response"></a><span data-ttu-id="63b7b-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="63b7b-164">Response</span></span>
<span data-ttu-id="63b7b-165">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63b7b-165">If successful, this method returns a `200 OK` response code and an updated [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63b7b-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63b7b-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="63b7b-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63b7b-167">Request</span></span>
<span data-ttu-id="63b7b-168">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63b7b-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="63b7b-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="63b7b-169">Response</span></span>
<span data-ttu-id="63b7b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="63b7b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




