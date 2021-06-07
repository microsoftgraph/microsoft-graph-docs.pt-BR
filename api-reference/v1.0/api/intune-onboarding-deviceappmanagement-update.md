---
title: Atualizar deviceAppManagement
description: Atualizar as propriedades de um objeto de deviceAppManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cc443e6f6d99a220c9e5b9a3bc88cd4cf30ec013
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759453"
---
# <a name="update-deviceappmanagement"></a><span data-ttu-id="60cba-103">Atualizar deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="60cba-103">Update deviceAppManagement</span></span>

<span data-ttu-id="60cba-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60cba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="60cba-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="60cba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60cba-106">Atualizar as propriedades de um objeto de [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="60cba-106">Update the properties of a [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60cba-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="60cba-107">Prerequisites</span></span>
<span data-ttu-id="60cba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60cba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60cba-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60cba-110">Permission type</span></span>|<span data-ttu-id="60cba-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="60cba-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60cba-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60cba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="60cba-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60cba-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="60cba-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60cba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60cba-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60cba-115">Not supported.</span></span>|
|<span data-ttu-id="60cba-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60cba-116">Application</span></span>|<span data-ttu-id="60cba-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60cba-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="60cba-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60cba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="60cba-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60cba-119">Request headers</span></span>
|<span data-ttu-id="60cba-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="60cba-120">Header</span></span>|<span data-ttu-id="60cba-121">Valor</span><span class="sxs-lookup"><span data-stu-id="60cba-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60cba-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="60cba-122">Authorization</span></span>|<span data-ttu-id="60cba-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60cba-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60cba-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="60cba-124">Accept</span></span>|<span data-ttu-id="60cba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="60cba-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60cba-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60cba-126">Request body</span></span>
<span data-ttu-id="60cba-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="60cba-127">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md) object.</span></span>

<span data-ttu-id="60cba-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="60cba-128">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md).</span></span>

|<span data-ttu-id="60cba-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60cba-129">Property</span></span>|<span data-ttu-id="60cba-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="60cba-130">Type</span></span>|<span data-ttu-id="60cba-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="60cba-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60cba-132">id</span><span class="sxs-lookup"><span data-stu-id="60cba-132">id</span></span>|<span data-ttu-id="60cba-133">String</span><span class="sxs-lookup"><span data-stu-id="60cba-133">String</span></span>|<span data-ttu-id="60cba-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="60cba-134">Not yet documented</span></span>|
|<span data-ttu-id="60cba-135">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="60cba-135">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="60cba-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60cba-136">DateTimeOffset</span></span>|<span data-ttu-id="60cba-137">A última vez que os aplicativos da Microsoft Store para Empresas foram sincronizados com êxito para essa conta.</span><span class="sxs-lookup"><span data-stu-id="60cba-137">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|
|<span data-ttu-id="60cba-138">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="60cba-138">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="60cba-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="60cba-139">Boolean</span></span>|<span data-ttu-id="60cba-140">Se a conta está ativada para sincronizar aplicativos do Microsoft Store para Empresa.</span><span class="sxs-lookup"><span data-stu-id="60cba-140">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="60cba-141">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="60cba-141">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="60cba-142">String</span><span class="sxs-lookup"><span data-stu-id="60cba-142">String</span></span>|<span data-ttu-id="60cba-143">As informações sobre a localidade usada para sincronizar aplicativos do Microsoft Store para Empresas.</span><span class="sxs-lookup"><span data-stu-id="60cba-143">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="60cba-144">Culturas específicas de um país/região.</span><span class="sxs-lookup"><span data-stu-id="60cba-144">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="60cba-145">Os nomes dessas culturas seguem a RFC 4646 (Windows Vista e mais recentes).</span><span class="sxs-lookup"><span data-stu-id="60cba-145">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="60cba-146">O formato é <languagecode2>-<country/regioncode2>, onde <languagecode2> é um código em duas letras minúsculas derivado da ISO 639-1 e <country/regioncode2> é um código em duas letras maiúsculas derivado da ISO 3166.</span><span class="sxs-lookup"><span data-stu-id="60cba-146">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="60cba-147">Por exemplo, en-US para inglês (Estados Unidos) é uma cultura específica.</span><span class="sxs-lookup"><span data-stu-id="60cba-147">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="60cba-148">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="60cba-148">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="60cba-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60cba-149">DateTimeOffset</span></span>|<span data-ttu-id="60cba-150">A última vez em uma sincronização de aplicativo na Microsoft Store para Empresas foi concluída.</span><span class="sxs-lookup"><span data-stu-id="60cba-150">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|



## <a name="response"></a><span data-ttu-id="60cba-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="60cba-151">Response</span></span>
<span data-ttu-id="60cba-152">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60cba-152">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60cba-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60cba-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="60cba-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60cba-154">Request</span></span>
<span data-ttu-id="60cba-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60cba-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 394

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "2016-12-31T23:57:45.2453148-08:00",
  "isEnabledForMicrosoftStoreForBusiness": true,
  "microsoftStoreForBusinessLanguage": "Microsoft Store For Business Language value",
  "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "2017-01-01T00:02:00.0421137-08:00"
}
```

### <a name="response"></a><span data-ttu-id="60cba-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="60cba-156">Response</span></span>
<span data-ttu-id="60cba-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60cba-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 443

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb",
  "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "2016-12-31T23:57:45.2453148-08:00",
  "isEnabledForMicrosoftStoreForBusiness": true,
  "microsoftStoreForBusinessLanguage": "Microsoft Store For Business Language value",
  "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "2017-01-01T00:02:00.0421137-08:00"
}
```




