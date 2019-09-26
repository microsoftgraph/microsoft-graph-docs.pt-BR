---
title: Criar dataSharingConsent
description: Criar um novo objeto dataSharingConsent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 873f0d5c91a571e71fc6f8d754742ecb51f9d049
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37180682"
---
# <a name="create-datasharingconsent"></a><span data-ttu-id="2ed87-103">Criar dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="2ed87-103">Create dataSharingConsent</span></span>

> <span data-ttu-id="2ed87-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2ed87-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ed87-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2ed87-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ed87-106">Criar um novo objeto [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) .</span><span class="sxs-lookup"><span data-stu-id="2ed87-106">Create a new [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ed87-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2ed87-107">Prerequisites</span></span>
<span data-ttu-id="2ed87-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ed87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ed87-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ed87-110">Permission type</span></span>|<span data-ttu-id="2ed87-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2ed87-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ed87-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ed87-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2ed87-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ed87-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2ed87-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ed87-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ed87-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ed87-115">Not supported.</span></span>|
|<span data-ttu-id="2ed87-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ed87-116">Application</span></span>|<span data-ttu-id="2ed87-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ed87-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ed87-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ed87-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/dataSharingConsents
```

## <a name="request-headers"></a><span data-ttu-id="2ed87-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ed87-119">Request headers</span></span>
|<span data-ttu-id="2ed87-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2ed87-120">Header</span></span>|<span data-ttu-id="2ed87-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2ed87-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ed87-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ed87-122">Authorization</span></span>|<span data-ttu-id="2ed87-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ed87-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ed87-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2ed87-124">Accept</span></span>|<span data-ttu-id="2ed87-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2ed87-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ed87-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ed87-126">Request body</span></span>
<span data-ttu-id="2ed87-127">No corpo da solicitação, forneça uma representação JSON do objeto dataSharingConsent.</span><span class="sxs-lookup"><span data-stu-id="2ed87-127">In the request body, supply a JSON representation for the dataSharingConsent object.</span></span>

<span data-ttu-id="2ed87-128">A tabela a seguir mostra as propriedades que são necessárias ao criar dataSharingConsent.</span><span class="sxs-lookup"><span data-stu-id="2ed87-128">The following table shows the properties that are required when you create the dataSharingConsent.</span></span>

|<span data-ttu-id="2ed87-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ed87-129">Property</span></span>|<span data-ttu-id="2ed87-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ed87-130">Type</span></span>|<span data-ttu-id="2ed87-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ed87-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ed87-132">id</span><span class="sxs-lookup"><span data-stu-id="2ed87-132">id</span></span>|<span data-ttu-id="2ed87-133">String</span><span class="sxs-lookup"><span data-stu-id="2ed87-133">String</span></span>|<span data-ttu-id="2ed87-134">A ID de consentimento de compartilhamento de dados</span><span class="sxs-lookup"><span data-stu-id="2ed87-134">The data sharing consent Id</span></span>|
|<span data-ttu-id="2ed87-135">objectdisplayname</span><span class="sxs-lookup"><span data-stu-id="2ed87-135">serviceDisplayName</span></span>|<span data-ttu-id="2ed87-136">String</span><span class="sxs-lookup"><span data-stu-id="2ed87-136">String</span></span>|<span data-ttu-id="2ed87-137">O nome de exibição do fluxo de trabalho do serviço</span><span class="sxs-lookup"><span data-stu-id="2ed87-137">The display name of the service work flow</span></span>|
|<span data-ttu-id="2ed87-138">termsUrl</span><span class="sxs-lookup"><span data-stu-id="2ed87-138">termsUrl</span></span>|<span data-ttu-id="2ed87-139">String</span><span class="sxs-lookup"><span data-stu-id="2ed87-139">String</span></span>|<span data-ttu-id="2ed87-140">O TermsUrl para o consentimento de compartilhamento de dados</span><span class="sxs-lookup"><span data-stu-id="2ed87-140">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="2ed87-141">granted</span><span class="sxs-lookup"><span data-stu-id="2ed87-141">granted</span></span>|<span data-ttu-id="2ed87-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="2ed87-142">Boolean</span></span>|<span data-ttu-id="2ed87-143">O Estado concedido para o consentimento de compartilhamento de dados</span><span class="sxs-lookup"><span data-stu-id="2ed87-143">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="2ed87-144">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="2ed87-144">grantDateTime</span></span>|<span data-ttu-id="2ed87-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ed87-145">DateTimeOffset</span></span>|<span data-ttu-id="2ed87-146">O consentimento de tempo foi concedido para esta conta</span><span class="sxs-lookup"><span data-stu-id="2ed87-146">The time consent was granted for this account</span></span>|
|<span data-ttu-id="2ed87-147">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="2ed87-147">grantedByUpn</span></span>|<span data-ttu-id="2ed87-148">String</span><span class="sxs-lookup"><span data-stu-id="2ed87-148">String</span></span>|<span data-ttu-id="2ed87-149">O UPN do usuário que concedeu o consentimento para esta conta</span><span class="sxs-lookup"><span data-stu-id="2ed87-149">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="2ed87-150">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="2ed87-150">grantedByUserId</span></span>|<span data-ttu-id="2ed87-151">String</span><span class="sxs-lookup"><span data-stu-id="2ed87-151">String</span></span>|<span data-ttu-id="2ed87-152">O UserId do usuário que concedeu o consentimento para esta conta</span><span class="sxs-lookup"><span data-stu-id="2ed87-152">The UserId of the user that granted consent for this account</span></span>|



## <a name="response"></a><span data-ttu-id="2ed87-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ed87-153">Response</span></span>
<span data-ttu-id="2ed87-154">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ed87-154">If successful, this method returns a `201 Created` response code and a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ed87-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ed87-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ed87-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ed87-156">Request</span></span>
<span data-ttu-id="2ed87-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ed87-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents
Content-type: application/json
Content-length: 333

{
  "@odata.type": "#microsoft.graph.dataSharingConsent",
  "serviceDisplayName": "Service Display Name value",
  "termsUrl": "https://example.com/termsUrl/",
  "granted": true,
  "grantDateTime": "2016-12-31T23:59:55.7154191-08:00",
  "grantedByUpn": "Granted By Upn value",
  "grantedByUserId": "Granted By User Id value"
}
```

### <a name="response"></a><span data-ttu-id="2ed87-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ed87-158">Response</span></span>
<span data-ttu-id="2ed87-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2ed87-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 382

{
  "@odata.type": "#microsoft.graph.dataSharingConsent",
  "id": "333387f7-87f7-3333-f787-3333f7873333",
  "serviceDisplayName": "Service Display Name value",
  "termsUrl": "https://example.com/termsUrl/",
  "granted": true,
  "grantDateTime": "2016-12-31T23:59:55.7154191-08:00",
  "grantedByUpn": "Granted By Upn value",
  "grantedByUserId": "Granted By User Id value"
}
```




