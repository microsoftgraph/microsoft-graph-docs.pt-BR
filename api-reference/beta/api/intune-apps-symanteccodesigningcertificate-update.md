---
title: Atualizar symantecCodeSigningCertificate
description: Atualize as propriedades de um objeto symantecCodeSigningCertificate.
ms.openlocfilehash: a6122997a4bc0c76521612b5b17a9c42cd944664
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039052"
---
# <a name="update-symanteccodesigningcertificate"></a><span data-ttu-id="8de9d-103">Atualizar symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="8de9d-103">Update symantecCodeSigningCertificate</span></span>

> <span data-ttu-id="8de9d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8de9d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8de9d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8de9d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8de9d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8de9d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8de9d-107">Atualize as propriedades de um objeto [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="8de9d-107">Update the properties of a [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8de9d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8de9d-108">Prerequisites</span></span>
<span data-ttu-id="8de9d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8de9d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8de9d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8de9d-111">Permission type</span></span>|<span data-ttu-id="8de9d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8de9d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8de9d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8de9d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8de9d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8de9d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8de9d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8de9d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8de9d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8de9d-116">Not supported.</span></span>|
|<span data-ttu-id="8de9d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8de9d-117">Application</span></span>|<span data-ttu-id="8de9d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8de9d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8de9d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8de9d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/symantecCodeSigningCertificate
```

## <a name="request-headers"></a><span data-ttu-id="8de9d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8de9d-120">Request headers</span></span>
|<span data-ttu-id="8de9d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8de9d-121">Header</span></span>|<span data-ttu-id="8de9d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8de9d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8de9d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8de9d-123">Authorization</span></span>|<span data-ttu-id="8de9d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8de9d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8de9d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8de9d-125">Accept</span></span>|<span data-ttu-id="8de9d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8de9d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8de9d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8de9d-127">Request body</span></span>
<span data-ttu-id="8de9d-128">No corpo da solicitação, fornece uma representação JSON para o objeto [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="8de9d-128">In the request body, supply a JSON representation for the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

<span data-ttu-id="8de9d-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="8de9d-129">The following table shows the properties that are required when you create the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md).</span></span>

|<span data-ttu-id="8de9d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8de9d-130">Property</span></span>|<span data-ttu-id="8de9d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8de9d-131">Type</span></span>|<span data-ttu-id="8de9d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8de9d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8de9d-133">id</span><span class="sxs-lookup"><span data-stu-id="8de9d-133">id</span></span>|<span data-ttu-id="8de9d-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8de9d-134">String</span></span>|<span data-ttu-id="8de9d-135">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8de9d-135">The key of the entity.</span></span>|
|<span data-ttu-id="8de9d-136">content</span><span class="sxs-lookup"><span data-stu-id="8de9d-136">content</span></span>|<span data-ttu-id="8de9d-137">Binário</span><span class="sxs-lookup"><span data-stu-id="8de9d-137">Binary</span></span>|<span data-ttu-id="8de9d-138">O certificado de assinatura de código do Windows Symantec no formato de dados brutos.</span><span class="sxs-lookup"><span data-stu-id="8de9d-138">The Windows Symantec Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="8de9d-139">status</span><span class="sxs-lookup"><span data-stu-id="8de9d-139">status</span></span>|[<span data-ttu-id="8de9d-140">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="8de9d-140">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="8de9d-141">O Status de Cert provisionado ou não foi provisionado.</span><span class="sxs-lookup"><span data-stu-id="8de9d-141">The Cert Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="8de9d-142">Os valores possíveis são: `notProvisioned` e `provisioned`.</span><span class="sxs-lookup"><span data-stu-id="8de9d-142">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="8de9d-143">password</span><span class="sxs-lookup"><span data-stu-id="8de9d-143">password</span></span>|<span data-ttu-id="8de9d-144">String</span><span class="sxs-lookup"><span data-stu-id="8de9d-144">String</span></span>|<span data-ttu-id="8de9d-145">A senha necessária para o arquivo. pfx.</span><span class="sxs-lookup"><span data-stu-id="8de9d-145">The Password required for .pfx file.</span></span>|
|<span data-ttu-id="8de9d-146">SubjectName</span><span class="sxs-lookup"><span data-stu-id="8de9d-146">subjectName</span></span>|<span data-ttu-id="8de9d-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8de9d-147">String</span></span>|<span data-ttu-id="8de9d-148">O nome do assunto para o cert.</span><span class="sxs-lookup"><span data-stu-id="8de9d-148">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="8de9d-149">subject</span><span class="sxs-lookup"><span data-stu-id="8de9d-149">subject</span></span>|<span data-ttu-id="8de9d-150">String</span><span class="sxs-lookup"><span data-stu-id="8de9d-150">String</span></span>|<span data-ttu-id="8de9d-151">O valor de assunto para o cert.</span><span class="sxs-lookup"><span data-stu-id="8de9d-151">The Subject value for the cert.</span></span>|
|<span data-ttu-id="8de9d-152">issuerName</span><span class="sxs-lookup"><span data-stu-id="8de9d-152">issuerName</span></span>|<span data-ttu-id="8de9d-153">String</span><span class="sxs-lookup"><span data-stu-id="8de9d-153">String</span></span>|<span data-ttu-id="8de9d-154">O nome do emissor para o cert.</span><span class="sxs-lookup"><span data-stu-id="8de9d-154">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="8de9d-155">emissor</span><span class="sxs-lookup"><span data-stu-id="8de9d-155">issuer</span></span>|<span data-ttu-id="8de9d-156">String</span><span class="sxs-lookup"><span data-stu-id="8de9d-156">String</span></span>|<span data-ttu-id="8de9d-157">O valor de emissor para o cert.</span><span class="sxs-lookup"><span data-stu-id="8de9d-157">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="8de9d-158">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8de9d-158">expirationDateTime</span></span>|<span data-ttu-id="8de9d-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8de9d-159">DateTimeOffset</span></span>|<span data-ttu-id="8de9d-160">A data de validade do Cert.</span><span class="sxs-lookup"><span data-stu-id="8de9d-160">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="8de9d-161">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="8de9d-161">uploadDateTime</span></span>|<span data-ttu-id="8de9d-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8de9d-162">DateTimeOffset</span></span>|<span data-ttu-id="8de9d-163">O tipo do certificado de assinatura de código padrão como Symantec Cert.</span><span class="sxs-lookup"><span data-stu-id="8de9d-163">The Type of the CodeSigning Cert as Symantec Cert.</span></span>|



## <a name="response"></a><span data-ttu-id="8de9d-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="8de9d-164">Response</span></span>
<span data-ttu-id="8de9d-165">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8de9d-165">If successful, this method returns a `200 OK` response code and an updated [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8de9d-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8de9d-166">Example</span></span>
### <a name="request"></a><span data-ttu-id="8de9d-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8de9d-167">Request</span></span>
<span data-ttu-id="8de9d-168">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8de9d-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/symantecCodeSigningCertificate
Content-type: application/json
Content-length: 352

{
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

### <a name="response"></a><span data-ttu-id="8de9d-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="8de9d-169">Response</span></span>
<span data-ttu-id="8de9d-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8de9d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





