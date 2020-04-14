---
title: Criar dataSharingConsent
description: Criar um novo objeto dataSharingConsent.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 57b109d806e8fd3b6ff510985666448a98dbcaee
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43426718"
---
# <a name="create-datasharingconsent"></a><span data-ttu-id="df8b6-103">Criar dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="df8b6-103">Create dataSharingConsent</span></span>

<span data-ttu-id="df8b6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df8b6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df8b6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="df8b6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df8b6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="df8b6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df8b6-107">Criar um novo objeto [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) .</span><span class="sxs-lookup"><span data-stu-id="df8b6-107">Create a new [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df8b6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="df8b6-108">Prerequisites</span></span>
<span data-ttu-id="df8b6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df8b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df8b6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df8b6-111">Permission type</span></span>|<span data-ttu-id="df8b6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="df8b6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df8b6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df8b6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="df8b6-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df8b6-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="df8b6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df8b6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df8b6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df8b6-116">Not supported.</span></span>|
|<span data-ttu-id="df8b6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df8b6-117">Application</span></span>|<span data-ttu-id="df8b6-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df8b6-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="df8b6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df8b6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/dataSharingConsents
```

## <a name="request-headers"></a><span data-ttu-id="df8b6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df8b6-120">Request headers</span></span>
|<span data-ttu-id="df8b6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="df8b6-121">Header</span></span>|<span data-ttu-id="df8b6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="df8b6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df8b6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="df8b6-123">Authorization</span></span>|<span data-ttu-id="df8b6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df8b6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df8b6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="df8b6-125">Accept</span></span>|<span data-ttu-id="df8b6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="df8b6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df8b6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df8b6-127">Request body</span></span>
<span data-ttu-id="df8b6-128">No corpo da solicitação, forneça uma representação JSON do objeto dataSharingConsent.</span><span class="sxs-lookup"><span data-stu-id="df8b6-128">In the request body, supply a JSON representation for the dataSharingConsent object.</span></span>

<span data-ttu-id="df8b6-129">A tabela a seguir mostra as propriedades que são necessárias ao criar dataSharingConsent.</span><span class="sxs-lookup"><span data-stu-id="df8b6-129">The following table shows the properties that are required when you create the dataSharingConsent.</span></span>

|<span data-ttu-id="df8b6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df8b6-130">Property</span></span>|<span data-ttu-id="df8b6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="df8b6-131">Type</span></span>|<span data-ttu-id="df8b6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="df8b6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df8b6-133">id</span><span class="sxs-lookup"><span data-stu-id="df8b6-133">id</span></span>|<span data-ttu-id="df8b6-134">String</span><span class="sxs-lookup"><span data-stu-id="df8b6-134">String</span></span>|<span data-ttu-id="df8b6-135">A ID de consentimento de compartilhamento de dados</span><span class="sxs-lookup"><span data-stu-id="df8b6-135">The data sharing consent Id</span></span>|
|<span data-ttu-id="df8b6-136">objectdisplayname</span><span class="sxs-lookup"><span data-stu-id="df8b6-136">serviceDisplayName</span></span>|<span data-ttu-id="df8b6-137">String</span><span class="sxs-lookup"><span data-stu-id="df8b6-137">String</span></span>|<span data-ttu-id="df8b6-138">O nome de exibição do fluxo de trabalho do serviço</span><span class="sxs-lookup"><span data-stu-id="df8b6-138">The display name of the service work flow</span></span>|
|<span data-ttu-id="df8b6-139">termsUrl</span><span class="sxs-lookup"><span data-stu-id="df8b6-139">termsUrl</span></span>|<span data-ttu-id="df8b6-140">String</span><span class="sxs-lookup"><span data-stu-id="df8b6-140">String</span></span>|<span data-ttu-id="df8b6-141">O TermsUrl para o consentimento de compartilhamento de dados</span><span class="sxs-lookup"><span data-stu-id="df8b6-141">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="df8b6-142">granted</span><span class="sxs-lookup"><span data-stu-id="df8b6-142">granted</span></span>|<span data-ttu-id="df8b6-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="df8b6-143">Boolean</span></span>|<span data-ttu-id="df8b6-144">O Estado concedido para o consentimento de compartilhamento de dados</span><span class="sxs-lookup"><span data-stu-id="df8b6-144">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="df8b6-145">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="df8b6-145">grantDateTime</span></span>|<span data-ttu-id="df8b6-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df8b6-146">DateTimeOffset</span></span>|<span data-ttu-id="df8b6-147">O consentimento de tempo foi concedido para esta conta</span><span class="sxs-lookup"><span data-stu-id="df8b6-147">The time consent was granted for this account</span></span>|
|<span data-ttu-id="df8b6-148">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="df8b6-148">grantedByUpn</span></span>|<span data-ttu-id="df8b6-149">String</span><span class="sxs-lookup"><span data-stu-id="df8b6-149">String</span></span>|<span data-ttu-id="df8b6-150">O UPN do usuário que concedeu o consentimento para esta conta</span><span class="sxs-lookup"><span data-stu-id="df8b6-150">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="df8b6-151">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="df8b6-151">grantedByUserId</span></span>|<span data-ttu-id="df8b6-152">String</span><span class="sxs-lookup"><span data-stu-id="df8b6-152">String</span></span>|<span data-ttu-id="df8b6-153">O UserId do usuário que concedeu o consentimento para esta conta</span><span class="sxs-lookup"><span data-stu-id="df8b6-153">The UserId of the user that granted consent for this account</span></span>|



## <a name="response"></a><span data-ttu-id="df8b6-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="df8b6-154">Response</span></span>
<span data-ttu-id="df8b6-155">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df8b6-155">If successful, this method returns a `201 Created` response code and a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df8b6-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df8b6-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="df8b6-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df8b6-157">Request</span></span>
<span data-ttu-id="df8b6-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="df8b6-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="df8b6-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="df8b6-159">Response</span></span>
<span data-ttu-id="df8b6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df8b6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



