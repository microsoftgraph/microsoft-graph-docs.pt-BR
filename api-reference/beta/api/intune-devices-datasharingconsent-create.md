---
title: Criar dataSharingConsent
description: Crie um novo objeto de dataSharingConsent.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 686f8e5ddb56c53224d467bc6ac31cfdb5b6858c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406945"
---
# <a name="create-datasharingconsent"></a><span data-ttu-id="7ab17-103">Criar dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="7ab17-103">Create dataSharingConsent</span></span>

> <span data-ttu-id="7ab17-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="7ab17-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7ab17-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7ab17-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7ab17-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="7ab17-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ab17-107">Crie um novo objeto de [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) .</span><span class="sxs-lookup"><span data-stu-id="7ab17-107">Create a new [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ab17-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7ab17-108">Prerequisites</span></span>
<span data-ttu-id="7ab17-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7ab17-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7ab17-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ab17-111">Permission type</span></span>|<span data-ttu-id="7ab17-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7ab17-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ab17-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ab17-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7ab17-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ab17-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7ab17-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ab17-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ab17-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ab17-116">Not supported.</span></span>|
|<span data-ttu-id="7ab17-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ab17-117">Application</span></span>|<span data-ttu-id="7ab17-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ab17-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ab17-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ab17-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/dataSharingConsents
```

## <a name="request-headers"></a><span data-ttu-id="7ab17-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ab17-120">Request headers</span></span>
|<span data-ttu-id="7ab17-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7ab17-121">Header</span></span>|<span data-ttu-id="7ab17-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7ab17-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ab17-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ab17-123">Authorization</span></span>|<span data-ttu-id="7ab17-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ab17-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ab17-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7ab17-125">Accept</span></span>|<span data-ttu-id="7ab17-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7ab17-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ab17-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ab17-127">Request body</span></span>
<span data-ttu-id="7ab17-128">No corpo da solicitação, fornece uma representação JSON para o objeto dataSharingConsent.</span><span class="sxs-lookup"><span data-stu-id="7ab17-128">In the request body, supply a JSON representation for the dataSharingConsent object.</span></span>

<span data-ttu-id="7ab17-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o dataSharingConsent.</span><span class="sxs-lookup"><span data-stu-id="7ab17-129">The following table shows the properties that are required when you create the dataSharingConsent.</span></span>

|<span data-ttu-id="7ab17-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ab17-130">Property</span></span>|<span data-ttu-id="7ab17-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ab17-131">Type</span></span>|<span data-ttu-id="7ab17-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ab17-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ab17-133">id</span><span class="sxs-lookup"><span data-stu-id="7ab17-133">id</span></span>|<span data-ttu-id="7ab17-134">String</span><span class="sxs-lookup"><span data-stu-id="7ab17-134">String</span></span>|<span data-ttu-id="7ab17-135">O consentimento de compartilhamento de dados Id</span><span class="sxs-lookup"><span data-stu-id="7ab17-135">The data sharing consent Id</span></span>|
|<span data-ttu-id="7ab17-136">Nome_para_exibição_do_serviço</span><span class="sxs-lookup"><span data-stu-id="7ab17-136">serviceDisplayName</span></span>|<span data-ttu-id="7ab17-137">String</span><span class="sxs-lookup"><span data-stu-id="7ab17-137">String</span></span>|<span data-ttu-id="7ab17-138">O nome para exibição do fluxo de trabalho de serviço</span><span class="sxs-lookup"><span data-stu-id="7ab17-138">The display name of the service work flow</span></span>|
|<span data-ttu-id="7ab17-139">termsUrl</span><span class="sxs-lookup"><span data-stu-id="7ab17-139">termsUrl</span></span>|<span data-ttu-id="7ab17-140">String</span><span class="sxs-lookup"><span data-stu-id="7ab17-140">String</span></span>|<span data-ttu-id="7ab17-141">O TermsUrl para os consentimento de compartilhamento de dados</span><span class="sxs-lookup"><span data-stu-id="7ab17-141">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="7ab17-142">concedido</span><span class="sxs-lookup"><span data-stu-id="7ab17-142">granted</span></span>|<span data-ttu-id="7ab17-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ab17-143">Boolean</span></span>|<span data-ttu-id="7ab17-144">O estado foram concedido para os consentimento de compartilhamento de dados</span><span class="sxs-lookup"><span data-stu-id="7ab17-144">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="7ab17-145">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="7ab17-145">grantDateTime</span></span>|<span data-ttu-id="7ab17-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ab17-146">DateTimeOffset</span></span>|<span data-ttu-id="7ab17-147">O consentimento de tempo foi concedido para esta conta</span><span class="sxs-lookup"><span data-stu-id="7ab17-147">The time consent was granted for this account</span></span>|
|<span data-ttu-id="7ab17-148">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="7ab17-148">grantedByUpn</span></span>|<span data-ttu-id="7ab17-149">String</span><span class="sxs-lookup"><span data-stu-id="7ab17-149">String</span></span>|<span data-ttu-id="7ab17-150">O Upn do usuário que tenha concedido consentimento para esta conta</span><span class="sxs-lookup"><span data-stu-id="7ab17-150">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="7ab17-151">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="7ab17-151">grantedByUserId</span></span>|<span data-ttu-id="7ab17-152">String</span><span class="sxs-lookup"><span data-stu-id="7ab17-152">String</span></span>|<span data-ttu-id="7ab17-153">A identificação do usuário do usuário que tenha concedido consentimento para esta conta</span><span class="sxs-lookup"><span data-stu-id="7ab17-153">The UserId of the user that granted consent for this account</span></span>|



## <a name="response"></a><span data-ttu-id="7ab17-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ab17-154">Response</span></span>
<span data-ttu-id="7ab17-155">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ab17-155">If successful, this method returns a `201 Created` response code and a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ab17-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7ab17-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ab17-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ab17-157">Request</span></span>
<span data-ttu-id="7ab17-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ab17-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7ab17-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ab17-159">Response</span></span>
<span data-ttu-id="7ab17-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7ab17-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




