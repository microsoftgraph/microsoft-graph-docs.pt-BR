---
title: Atualizar enterpriseCodeSigningCertificate
description: Atualize as propriedades de um objeto enterpriseCodeSigningCertificate.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5272c0ff0e18fd7200e85ff51575c10825dbf7f5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829313"
---
# <a name="update-enterprisecodesigningcertificate"></a><span data-ttu-id="2bdcc-103">Atualizar enterpriseCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="2bdcc-103">Update enterpriseCodeSigningCertificate</span></span>

> <span data-ttu-id="2bdcc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2bdcc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2bdcc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2bdcc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2bdcc-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2bdcc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2bdcc-107">Atualize as propriedades de um objeto [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="2bdcc-107">Update the properties of a [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2bdcc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2bdcc-108">Prerequisites</span></span>
<span data-ttu-id="2bdcc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2bdcc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bdcc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2bdcc-111">Permission type</span></span>|<span data-ttu-id="2bdcc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2bdcc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2bdcc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2bdcc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2bdcc-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bdcc-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2bdcc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2bdcc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2bdcc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2bdcc-116">Not supported.</span></span>|
|<span data-ttu-id="2bdcc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2bdcc-117">Application</span></span>|<span data-ttu-id="2bdcc-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2bdcc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2bdcc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2bdcc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="2bdcc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2bdcc-120">Request headers</span></span>
|<span data-ttu-id="2bdcc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2bdcc-121">Header</span></span>|<span data-ttu-id="2bdcc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2bdcc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2bdcc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2bdcc-123">Authorization</span></span>|<span data-ttu-id="2bdcc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2bdcc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2bdcc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2bdcc-125">Accept</span></span>|<span data-ttu-id="2bdcc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2bdcc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bdcc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2bdcc-127">Request body</span></span>
<span data-ttu-id="2bdcc-128">No corpo da solicitação, fornece uma representação JSON para o objeto [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="2bdcc-128">In the request body, supply a JSON representation for the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

<span data-ttu-id="2bdcc-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="2bdcc-129">The following table shows the properties that are required when you create the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md).</span></span>

|<span data-ttu-id="2bdcc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2bdcc-130">Property</span></span>|<span data-ttu-id="2bdcc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2bdcc-131">Type</span></span>|<span data-ttu-id="2bdcc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2bdcc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bdcc-133">id</span><span class="sxs-lookup"><span data-stu-id="2bdcc-133">id</span></span>|<span data-ttu-id="2bdcc-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2bdcc-134">String</span></span>|<span data-ttu-id="2bdcc-135">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2bdcc-135">The key of the entity.</span></span>|
|<span data-ttu-id="2bdcc-136">content</span><span class="sxs-lookup"><span data-stu-id="2bdcc-136">content</span></span>|<span data-ttu-id="2bdcc-137">Binária</span><span class="sxs-lookup"><span data-stu-id="2bdcc-137">Binary</span></span>|<span data-ttu-id="2bdcc-138">O certificado de assinatura de código de empresa do Windows no formato de dados brutos.</span><span class="sxs-lookup"><span data-stu-id="2bdcc-138">The Windows Enterprise Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="2bdcc-139">status</span><span class="sxs-lookup"><span data-stu-id="2bdcc-139">status</span></span>|[<span data-ttu-id="2bdcc-140">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="2bdcc-140">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="2bdcc-141">O Status do certificado provisionado ou não foi provisionado.</span><span class="sxs-lookup"><span data-stu-id="2bdcc-141">The Certificate Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="2bdcc-142">Os valores possíveis são: `notProvisioned` e `provisioned`.</span><span class="sxs-lookup"><span data-stu-id="2bdcc-142">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="2bdcc-143">SubjectName</span><span class="sxs-lookup"><span data-stu-id="2bdcc-143">subjectName</span></span>|<span data-ttu-id="2bdcc-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2bdcc-144">String</span></span>|<span data-ttu-id="2bdcc-145">O nome do assunto para o cert.</span><span class="sxs-lookup"><span data-stu-id="2bdcc-145">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="2bdcc-146">subject</span><span class="sxs-lookup"><span data-stu-id="2bdcc-146">subject</span></span>|<span data-ttu-id="2bdcc-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2bdcc-147">String</span></span>|<span data-ttu-id="2bdcc-148">O valor de assunto para o cert.</span><span class="sxs-lookup"><span data-stu-id="2bdcc-148">The Subject Value for the cert.</span></span>|
|<span data-ttu-id="2bdcc-149">issuerName</span><span class="sxs-lookup"><span data-stu-id="2bdcc-149">issuerName</span></span>|<span data-ttu-id="2bdcc-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2bdcc-150">String</span></span>|<span data-ttu-id="2bdcc-151">O nome do emissor para o cert.</span><span class="sxs-lookup"><span data-stu-id="2bdcc-151">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="2bdcc-152">emissor</span><span class="sxs-lookup"><span data-stu-id="2bdcc-152">issuer</span></span>|<span data-ttu-id="2bdcc-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2bdcc-153">String</span></span>|<span data-ttu-id="2bdcc-154">O valor de emissor para o cert.</span><span class="sxs-lookup"><span data-stu-id="2bdcc-154">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="2bdcc-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2bdcc-155">expirationDateTime</span></span>|<span data-ttu-id="2bdcc-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2bdcc-156">DateTimeOffset</span></span>|<span data-ttu-id="2bdcc-157">A data de validade do Cert.</span><span class="sxs-lookup"><span data-stu-id="2bdcc-157">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="2bdcc-158">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="2bdcc-158">uploadDateTime</span></span>|<span data-ttu-id="2bdcc-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2bdcc-159">DateTimeOffset</span></span>|<span data-ttu-id="2bdcc-160">A data hora de certificado de assinatura de código padrão quando ele é carregado.</span><span class="sxs-lookup"><span data-stu-id="2bdcc-160">The date time of CodeSigning Cert when it is uploaded.</span></span>|



## <a name="response"></a><span data-ttu-id="2bdcc-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bdcc-161">Response</span></span>
<span data-ttu-id="2bdcc-162">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2bdcc-162">If successful, this method returns a `200 OK` response code and an updated [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2bdcc-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2bdcc-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="2bdcc-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2bdcc-164">Request</span></span>
<span data-ttu-id="2bdcc-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2bdcc-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
Content-type: application/json
Content-length: 319

{
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

### <a name="response"></a><span data-ttu-id="2bdcc-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bdcc-166">Response</span></span>
<span data-ttu-id="2bdcc-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2bdcc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





