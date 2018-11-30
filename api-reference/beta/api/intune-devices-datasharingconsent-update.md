---
title: Atualizar dataSharingConsent
description: Atualize as propriedades de um objeto dataSharingConsent.
ms.openlocfilehash: 75cf844a279bf45dc5297b08a3926031b8cdc06a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039195"
---
# <a name="update-datasharingconsent"></a><span data-ttu-id="33a0a-103">Atualizar dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="33a0a-103">Update dataSharingConsent</span></span>

> <span data-ttu-id="33a0a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="33a0a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="33a0a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="33a0a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="33a0a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="33a0a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="33a0a-107">Atualize as propriedades de um objeto [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) .</span><span class="sxs-lookup"><span data-stu-id="33a0a-107">Update the properties of a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="33a0a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="33a0a-108">Prerequisites</span></span>
<span data-ttu-id="33a0a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33a0a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33a0a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33a0a-111">Permission type</span></span>|<span data-ttu-id="33a0a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="33a0a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33a0a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33a0a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="33a0a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33a0a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="33a0a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33a0a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33a0a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33a0a-116">Not supported.</span></span>|
|<span data-ttu-id="33a0a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33a0a-117">Application</span></span>|<span data-ttu-id="33a0a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33a0a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33a0a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33a0a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/dataSharingConsents/{dataSharingConsentId}
```

## <a name="request-headers"></a><span data-ttu-id="33a0a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33a0a-120">Request headers</span></span>
|<span data-ttu-id="33a0a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="33a0a-121">Header</span></span>|<span data-ttu-id="33a0a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="33a0a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33a0a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="33a0a-123">Authorization</span></span>|<span data-ttu-id="33a0a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33a0a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33a0a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="33a0a-125">Accept</span></span>|<span data-ttu-id="33a0a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="33a0a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33a0a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33a0a-127">Request body</span></span>
<span data-ttu-id="33a0a-128">No corpo da solicitação, fornece uma representação JSON para o objeto [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) .</span><span class="sxs-lookup"><span data-stu-id="33a0a-128">In the request body, supply a JSON representation for the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

<span data-ttu-id="33a0a-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).</span><span class="sxs-lookup"><span data-stu-id="33a0a-129">The following table shows the properties that are required when you create the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).</span></span>

|<span data-ttu-id="33a0a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33a0a-130">Property</span></span>|<span data-ttu-id="33a0a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="33a0a-131">Type</span></span>|<span data-ttu-id="33a0a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="33a0a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33a0a-133">id</span><span class="sxs-lookup"><span data-stu-id="33a0a-133">id</span></span>|<span data-ttu-id="33a0a-134">String</span><span class="sxs-lookup"><span data-stu-id="33a0a-134">String</span></span>|<span data-ttu-id="33a0a-135">O consentimento de compartilhamento de dados Id</span><span class="sxs-lookup"><span data-stu-id="33a0a-135">The data sharing consent Id</span></span>|
|<span data-ttu-id="33a0a-136">Nome_para_exibição_do_serviço</span><span class="sxs-lookup"><span data-stu-id="33a0a-136">serviceDisplayName</span></span>|<span data-ttu-id="33a0a-137">String</span><span class="sxs-lookup"><span data-stu-id="33a0a-137">String</span></span>|<span data-ttu-id="33a0a-138">O nome para exibição do fluxo de trabalho de serviço</span><span class="sxs-lookup"><span data-stu-id="33a0a-138">The display name of the service work flow</span></span>|
|<span data-ttu-id="33a0a-139">termsUrl</span><span class="sxs-lookup"><span data-stu-id="33a0a-139">termsUrl</span></span>|<span data-ttu-id="33a0a-140">String</span><span class="sxs-lookup"><span data-stu-id="33a0a-140">String</span></span>|<span data-ttu-id="33a0a-141">O TermsUrl para os consentimento de compartilhamento de dados</span><span class="sxs-lookup"><span data-stu-id="33a0a-141">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="33a0a-142">concedido</span><span class="sxs-lookup"><span data-stu-id="33a0a-142">granted</span></span>|<span data-ttu-id="33a0a-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="33a0a-143">Boolean</span></span>|<span data-ttu-id="33a0a-144">O estado foram concedido para os consentimento de compartilhamento de dados</span><span class="sxs-lookup"><span data-stu-id="33a0a-144">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="33a0a-145">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="33a0a-145">grantDateTime</span></span>|<span data-ttu-id="33a0a-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33a0a-146">DateTimeOffset</span></span>|<span data-ttu-id="33a0a-147">O consentimento de tempo foi concedido para esta conta</span><span class="sxs-lookup"><span data-stu-id="33a0a-147">The time consent was granted for this account</span></span>|
|<span data-ttu-id="33a0a-148">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="33a0a-148">grantedByUpn</span></span>|<span data-ttu-id="33a0a-149">String</span><span class="sxs-lookup"><span data-stu-id="33a0a-149">String</span></span>|<span data-ttu-id="33a0a-150">O Upn do usuário que tenha concedido consentimento para esta conta</span><span class="sxs-lookup"><span data-stu-id="33a0a-150">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="33a0a-151">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="33a0a-151">grantedByUserId</span></span>|<span data-ttu-id="33a0a-152">String</span><span class="sxs-lookup"><span data-stu-id="33a0a-152">String</span></span>|<span data-ttu-id="33a0a-153">A identificação do usuário do usuário que tenha concedido consentimento para esta conta</span><span class="sxs-lookup"><span data-stu-id="33a0a-153">The UserId of the user that granted consent for this account</span></span>|



## <a name="response"></a><span data-ttu-id="33a0a-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="33a0a-154">Response</span></span>
<span data-ttu-id="33a0a-155">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33a0a-155">If successful, this method returns a `200 OK` response code and an updated [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33a0a-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="33a0a-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="33a0a-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33a0a-157">Request</span></span>
<span data-ttu-id="33a0a-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="33a0a-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents/{dataSharingConsentId}
Content-type: application/json
Content-length: 276

{
  "serviceDisplayName": "Service Display Name value",
  "termsUrl": "https://example.com/termsUrl/",
  "granted": true,
  "grantDateTime": "2016-12-31T23:59:55.7154191-08:00",
  "grantedByUpn": "Granted By Upn value",
  "grantedByUserId": "Granted By User Id value"
}
```

### <a name="response"></a><span data-ttu-id="33a0a-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="33a0a-159">Response</span></span>
<span data-ttu-id="33a0a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="33a0a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





