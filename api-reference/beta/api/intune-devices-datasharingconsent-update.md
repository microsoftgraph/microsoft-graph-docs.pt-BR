---
title: Atualizar dataSharingConsent
description: Atualiza as propriedades de um objeto dataSharingConsent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5c90f9188af9c704929692c4b2ae32911022b319
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48698684"
---
# <a name="update-datasharingconsent"></a><span data-ttu-id="912a1-103">Atualizar dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="912a1-103">Update dataSharingConsent</span></span>

<span data-ttu-id="912a1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="912a1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="912a1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="912a1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="912a1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="912a1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="912a1-107">Atualiza as propriedades de um objeto [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) .</span><span class="sxs-lookup"><span data-stu-id="912a1-107">Update the properties of a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="912a1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="912a1-108">Prerequisites</span></span>
<span data-ttu-id="912a1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="912a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="912a1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="912a1-111">Permission type</span></span>|<span data-ttu-id="912a1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="912a1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="912a1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="912a1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="912a1-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="912a1-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="912a1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="912a1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="912a1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="912a1-116">Not supported.</span></span>|
|<span data-ttu-id="912a1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="912a1-117">Application</span></span>|<span data-ttu-id="912a1-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="912a1-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="912a1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="912a1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/dataSharingConsents/{dataSharingConsentId}
```

## <a name="request-headers"></a><span data-ttu-id="912a1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="912a1-120">Request headers</span></span>
|<span data-ttu-id="912a1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="912a1-121">Header</span></span>|<span data-ttu-id="912a1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="912a1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="912a1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="912a1-123">Authorization</span></span>|<span data-ttu-id="912a1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="912a1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="912a1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="912a1-125">Accept</span></span>|<span data-ttu-id="912a1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="912a1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="912a1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="912a1-127">Request body</span></span>
<span data-ttu-id="912a1-128">No corpo da solicitação, forneça uma representação JSON do objeto [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) .</span><span class="sxs-lookup"><span data-stu-id="912a1-128">In the request body, supply a JSON representation for the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

<span data-ttu-id="912a1-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).</span><span class="sxs-lookup"><span data-stu-id="912a1-129">The following table shows the properties that are required when you create the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).</span></span>

|<span data-ttu-id="912a1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="912a1-130">Property</span></span>|<span data-ttu-id="912a1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="912a1-131">Type</span></span>|<span data-ttu-id="912a1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="912a1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="912a1-133">id</span><span class="sxs-lookup"><span data-stu-id="912a1-133">id</span></span>|<span data-ttu-id="912a1-134">String</span><span class="sxs-lookup"><span data-stu-id="912a1-134">String</span></span>|<span data-ttu-id="912a1-135">A ID de consentimento de compartilhamento de dados</span><span class="sxs-lookup"><span data-stu-id="912a1-135">The data sharing consent Id</span></span>|
|<span data-ttu-id="912a1-136">objectdisplayname</span><span class="sxs-lookup"><span data-stu-id="912a1-136">serviceDisplayName</span></span>|<span data-ttu-id="912a1-137">String</span><span class="sxs-lookup"><span data-stu-id="912a1-137">String</span></span>|<span data-ttu-id="912a1-138">O nome de exibição do fluxo de trabalho do serviço</span><span class="sxs-lookup"><span data-stu-id="912a1-138">The display name of the service work flow</span></span>|
|<span data-ttu-id="912a1-139">termsUrl</span><span class="sxs-lookup"><span data-stu-id="912a1-139">termsUrl</span></span>|<span data-ttu-id="912a1-140">String</span><span class="sxs-lookup"><span data-stu-id="912a1-140">String</span></span>|<span data-ttu-id="912a1-141">O TermsUrl para o consentimento de compartilhamento de dados</span><span class="sxs-lookup"><span data-stu-id="912a1-141">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="912a1-142">granted</span><span class="sxs-lookup"><span data-stu-id="912a1-142">granted</span></span>|<span data-ttu-id="912a1-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="912a1-143">Boolean</span></span>|<span data-ttu-id="912a1-144">O Estado concedido para o consentimento de compartilhamento de dados</span><span class="sxs-lookup"><span data-stu-id="912a1-144">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="912a1-145">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="912a1-145">grantDateTime</span></span>|<span data-ttu-id="912a1-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="912a1-146">DateTimeOffset</span></span>|<span data-ttu-id="912a1-147">O consentimento de tempo foi concedido para esta conta</span><span class="sxs-lookup"><span data-stu-id="912a1-147">The time consent was granted for this account</span></span>|
|<span data-ttu-id="912a1-148">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="912a1-148">grantedByUpn</span></span>|<span data-ttu-id="912a1-149">String</span><span class="sxs-lookup"><span data-stu-id="912a1-149">String</span></span>|<span data-ttu-id="912a1-150">O UPN do usuário que concedeu o consentimento para esta conta</span><span class="sxs-lookup"><span data-stu-id="912a1-150">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="912a1-151">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="912a1-151">grantedByUserId</span></span>|<span data-ttu-id="912a1-152">String</span><span class="sxs-lookup"><span data-stu-id="912a1-152">String</span></span>|<span data-ttu-id="912a1-153">O UserId do usuário que concedeu o consentimento para esta conta</span><span class="sxs-lookup"><span data-stu-id="912a1-153">The UserId of the user that granted consent for this account</span></span>|



## <a name="response"></a><span data-ttu-id="912a1-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="912a1-154">Response</span></span>
<span data-ttu-id="912a1-155">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="912a1-155">If successful, this method returns a `200 OK` response code and an updated [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="912a1-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="912a1-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="912a1-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="912a1-157">Request</span></span>
<span data-ttu-id="912a1-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="912a1-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents/{dataSharingConsentId}
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

### <a name="response"></a><span data-ttu-id="912a1-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="912a1-159">Response</span></span>
<span data-ttu-id="912a1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="912a1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





