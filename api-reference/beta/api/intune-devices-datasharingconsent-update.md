---
title: Atualizar dataSharingConsent
description: Atualize as propriedades de um objeto dataSharingConsent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0d617546464b1333af2b535bbc1c17f61fa03386
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146542"
---
# <a name="update-datasharingconsent"></a><span data-ttu-id="79bc1-103">Atualizar dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="79bc1-103">Update dataSharingConsent</span></span>

<span data-ttu-id="79bc1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79bc1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="79bc1-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="79bc1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79bc1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="79bc1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79bc1-107">Atualize as propriedades de [um objeto dataSharingConsent.](../resources/intune-devices-datasharingconsent.md)</span><span class="sxs-lookup"><span data-stu-id="79bc1-107">Update the properties of a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79bc1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="79bc1-108">Prerequisites</span></span>
<span data-ttu-id="79bc1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79bc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79bc1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79bc1-111">Permission type</span></span>|<span data-ttu-id="79bc1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="79bc1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79bc1-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79bc1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="79bc1-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79bc1-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="79bc1-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79bc1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79bc1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79bc1-116">Not supported.</span></span>|
|<span data-ttu-id="79bc1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79bc1-117">Application</span></span>|<span data-ttu-id="79bc1-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79bc1-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79bc1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79bc1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/dataSharingConsents/{dataSharingConsentId}
```

## <a name="request-headers"></a><span data-ttu-id="79bc1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79bc1-120">Request headers</span></span>
|<span data-ttu-id="79bc1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="79bc1-121">Header</span></span>|<span data-ttu-id="79bc1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="79bc1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79bc1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="79bc1-123">Authorization</span></span>|<span data-ttu-id="79bc1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79bc1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79bc1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="79bc1-125">Accept</span></span>|<span data-ttu-id="79bc1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="79bc1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79bc1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79bc1-127">Request body</span></span>
<span data-ttu-id="79bc1-128">No corpo da solicitação, fornece uma representação JSON para o [objeto dataSharingConsent.](../resources/intune-devices-datasharingconsent.md)</span><span class="sxs-lookup"><span data-stu-id="79bc1-128">In the request body, supply a JSON representation for the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

<span data-ttu-id="79bc1-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o dataSharingConsent](../resources/intune-devices-datasharingconsent.md).</span><span class="sxs-lookup"><span data-stu-id="79bc1-129">The following table shows the properties that are required when you create the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).</span></span>

|<span data-ttu-id="79bc1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79bc1-130">Property</span></span>|<span data-ttu-id="79bc1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="79bc1-131">Type</span></span>|<span data-ttu-id="79bc1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="79bc1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79bc1-133">id</span><span class="sxs-lookup"><span data-stu-id="79bc1-133">id</span></span>|<span data-ttu-id="79bc1-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79bc1-134">String</span></span>|<span data-ttu-id="79bc1-135">A ID de consentimento de compartilhamento de dados</span><span class="sxs-lookup"><span data-stu-id="79bc1-135">The data sharing consent Id</span></span>|
|<span data-ttu-id="79bc1-136">serviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="79bc1-136">serviceDisplayName</span></span>|<span data-ttu-id="79bc1-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79bc1-137">String</span></span>|<span data-ttu-id="79bc1-138">O nome de exibição do fluxo de trabalho do serviço</span><span class="sxs-lookup"><span data-stu-id="79bc1-138">The display name of the service work flow</span></span>|
|<span data-ttu-id="79bc1-139">termsUrl</span><span class="sxs-lookup"><span data-stu-id="79bc1-139">termsUrl</span></span>|<span data-ttu-id="79bc1-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79bc1-140">String</span></span>|<span data-ttu-id="79bc1-141">The TermsUrl for the data sharing consent</span><span class="sxs-lookup"><span data-stu-id="79bc1-141">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="79bc1-142">concedido</span><span class="sxs-lookup"><span data-stu-id="79bc1-142">granted</span></span>|<span data-ttu-id="79bc1-143">Booleano</span><span class="sxs-lookup"><span data-stu-id="79bc1-143">Boolean</span></span>|<span data-ttu-id="79bc1-144">O estado concedido para o consentimento de compartilhamento de dados</span><span class="sxs-lookup"><span data-stu-id="79bc1-144">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="79bc1-145">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="79bc1-145">grantDateTime</span></span>|<span data-ttu-id="79bc1-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79bc1-146">DateTimeOffset</span></span>|<span data-ttu-id="79bc1-147">O consentimento de hora foi concedido para essa conta</span><span class="sxs-lookup"><span data-stu-id="79bc1-147">The time consent was granted for this account</span></span>|
|<span data-ttu-id="79bc1-148">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="79bc1-148">grantedByUpn</span></span>|<span data-ttu-id="79bc1-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79bc1-149">String</span></span>|<span data-ttu-id="79bc1-150">O Upn do usuário que concedeu consentimento para essa conta</span><span class="sxs-lookup"><span data-stu-id="79bc1-150">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="79bc1-151">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="79bc1-151">grantedByUserId</span></span>|<span data-ttu-id="79bc1-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79bc1-152">String</span></span>|<span data-ttu-id="79bc1-153">UserId do usuário que concedeu consentimento para essa conta</span><span class="sxs-lookup"><span data-stu-id="79bc1-153">The UserId of the user that granted consent for this account</span></span>|



## <a name="response"></a><span data-ttu-id="79bc1-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="79bc1-154">Response</span></span>
<span data-ttu-id="79bc1-155">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto dataSharingConsent](../resources/intune-devices-datasharingconsent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79bc1-155">If successful, this method returns a `200 OK` response code and an updated [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79bc1-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="79bc1-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="79bc1-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79bc1-157">Request</span></span>
<span data-ttu-id="79bc1-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="79bc1-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="79bc1-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="79bc1-159">Response</span></span>
<span data-ttu-id="79bc1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="79bc1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




