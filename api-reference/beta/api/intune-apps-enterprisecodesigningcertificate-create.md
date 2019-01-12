---
title: Criar enterpriseCodeSigningCertificate
description: Crie um novo objeto de enterpriseCodeSigningCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 302c10d1e0fbc5e182180a32ad96d614555d1d04
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956189"
---
# <a name="create-enterprisecodesigningcertificate"></a><span data-ttu-id="b762f-103">Criar enterpriseCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="b762f-103">Create enterpriseCodeSigningCertificate</span></span>

> <span data-ttu-id="b762f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b762f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b762f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b762f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b762f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b762f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b762f-107">Crie um novo objeto de [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="b762f-107">Create a new [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b762f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b762f-108">Prerequisites</span></span>
<span data-ttu-id="b762f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b762f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b762f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b762f-111">Permission type</span></span>|<span data-ttu-id="b762f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b762f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b762f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b762f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b762f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b762f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b762f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b762f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b762f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b762f-116">Not supported.</span></span>|
|<span data-ttu-id="b762f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b762f-117">Application</span></span>|<span data-ttu-id="b762f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b762f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b762f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b762f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/enterpriseCodeSigningCertificates
```

## <a name="request-headers"></a><span data-ttu-id="b762f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b762f-120">Request headers</span></span>
|<span data-ttu-id="b762f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b762f-121">Header</span></span>|<span data-ttu-id="b762f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b762f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b762f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b762f-123">Authorization</span></span>|<span data-ttu-id="b762f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b762f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b762f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b762f-125">Accept</span></span>|<span data-ttu-id="b762f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b762f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b762f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b762f-127">Request body</span></span>
<span data-ttu-id="b762f-128">No corpo da solicitação, fornece uma representação JSON para o objeto enterpriseCodeSigningCertificate.</span><span class="sxs-lookup"><span data-stu-id="b762f-128">In the request body, supply a JSON representation for the enterpriseCodeSigningCertificate object.</span></span>

<span data-ttu-id="b762f-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o enterpriseCodeSigningCertificate.</span><span class="sxs-lookup"><span data-stu-id="b762f-129">The following table shows the properties that are required when you create the enterpriseCodeSigningCertificate.</span></span>

|<span data-ttu-id="b762f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b762f-130">Property</span></span>|<span data-ttu-id="b762f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b762f-131">Type</span></span>|<span data-ttu-id="b762f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b762f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b762f-133">id</span><span class="sxs-lookup"><span data-stu-id="b762f-133">id</span></span>|<span data-ttu-id="b762f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b762f-134">String</span></span>|<span data-ttu-id="b762f-135">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b762f-135">The key of the entity.</span></span>|
|<span data-ttu-id="b762f-136">content</span><span class="sxs-lookup"><span data-stu-id="b762f-136">content</span></span>|<span data-ttu-id="b762f-137">Binária</span><span class="sxs-lookup"><span data-stu-id="b762f-137">Binary</span></span>|<span data-ttu-id="b762f-138">O certificado de assinatura de código de empresa do Windows no formato de dados brutos.</span><span class="sxs-lookup"><span data-stu-id="b762f-138">The Windows Enterprise Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="b762f-139">status</span><span class="sxs-lookup"><span data-stu-id="b762f-139">status</span></span>|[<span data-ttu-id="b762f-140">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="b762f-140">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="b762f-141">O Status do certificado provisionado ou não foi provisionado.</span><span class="sxs-lookup"><span data-stu-id="b762f-141">The Certificate Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="b762f-142">Os valores possíveis são: `notProvisioned` e `provisioned`.</span><span class="sxs-lookup"><span data-stu-id="b762f-142">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="b762f-143">SubjectName</span><span class="sxs-lookup"><span data-stu-id="b762f-143">subjectName</span></span>|<span data-ttu-id="b762f-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b762f-144">String</span></span>|<span data-ttu-id="b762f-145">O nome do assunto para o cert.</span><span class="sxs-lookup"><span data-stu-id="b762f-145">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="b762f-146">subject</span><span class="sxs-lookup"><span data-stu-id="b762f-146">subject</span></span>|<span data-ttu-id="b762f-147">String</span><span class="sxs-lookup"><span data-stu-id="b762f-147">String</span></span>|<span data-ttu-id="b762f-148">O valor de assunto para o cert.</span><span class="sxs-lookup"><span data-stu-id="b762f-148">The Subject Value for the cert.</span></span>|
|<span data-ttu-id="b762f-149">issuerName</span><span class="sxs-lookup"><span data-stu-id="b762f-149">issuerName</span></span>|<span data-ttu-id="b762f-150">String</span><span class="sxs-lookup"><span data-stu-id="b762f-150">String</span></span>|<span data-ttu-id="b762f-151">O nome do emissor para o cert.</span><span class="sxs-lookup"><span data-stu-id="b762f-151">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="b762f-152">emissor</span><span class="sxs-lookup"><span data-stu-id="b762f-152">issuer</span></span>|<span data-ttu-id="b762f-153">String</span><span class="sxs-lookup"><span data-stu-id="b762f-153">String</span></span>|<span data-ttu-id="b762f-154">O valor de emissor para o cert.</span><span class="sxs-lookup"><span data-stu-id="b762f-154">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="b762f-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b762f-155">expirationDateTime</span></span>|<span data-ttu-id="b762f-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b762f-156">DateTimeOffset</span></span>|<span data-ttu-id="b762f-157">A data de validade do Cert.</span><span class="sxs-lookup"><span data-stu-id="b762f-157">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="b762f-158">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="b762f-158">uploadDateTime</span></span>|<span data-ttu-id="b762f-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b762f-159">DateTimeOffset</span></span>|<span data-ttu-id="b762f-160">A data hora de certificado de assinatura de código padrão quando ele é carregado.</span><span class="sxs-lookup"><span data-stu-id="b762f-160">The date time of CodeSigning Cert when it is uploaded.</span></span>|



## <a name="response"></a><span data-ttu-id="b762f-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="b762f-161">Response</span></span>
<span data-ttu-id="b762f-162">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b762f-162">If successful, this method returns a `201 Created` response code and a [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b762f-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b762f-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="b762f-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b762f-164">Request</span></span>
<span data-ttu-id="b762f-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b762f-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b762f-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="b762f-166">Response</span></span>
<span data-ttu-id="b762f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b762f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





