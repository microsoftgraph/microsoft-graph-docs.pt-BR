---
title: Atualizar deviceAppManagement
description: Atualizar as propriedades de um objeto de deviceAppManagement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f97316e06cec39cd0aeb1b22d6142925d81b77ae
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259364"
---
# <a name="update-deviceappmanagement"></a><span data-ttu-id="176b2-103">Atualizar deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="176b2-103">Update deviceAppManagement</span></span>

> <span data-ttu-id="176b2-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="176b2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="176b2-105">Atualizar as propriedades de um objeto de [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="176b2-105">Update the properties of a [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="176b2-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="176b2-106">Prerequisites</span></span>
<span data-ttu-id="176b2-107">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="176b2-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="176b2-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="176b2-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="176b2-109">Observe que a permissão adequada varia de acordo com o fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="176b2-109">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="176b2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="176b2-110">Permission type</span></span>|<span data-ttu-id="176b2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="176b2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="176b2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="176b2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="176b2-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="176b2-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="176b2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="176b2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="176b2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="176b2-115">Not supported.</span></span>|
|<span data-ttu-id="176b2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="176b2-116">Application</span></span>|<span data-ttu-id="176b2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="176b2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="176b2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="176b2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="176b2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="176b2-119">Request headers</span></span>
|<span data-ttu-id="176b2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="176b2-120">Header</span></span>|<span data-ttu-id="176b2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="176b2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="176b2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="176b2-122">Authorization</span></span>|<span data-ttu-id="176b2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="176b2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="176b2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="176b2-124">Accept</span></span>|<span data-ttu-id="176b2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="176b2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="176b2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="176b2-126">Request body</span></span>
<span data-ttu-id="176b2-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="176b2-127">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

<span data-ttu-id="176b2-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="176b2-128">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span></span>

|<span data-ttu-id="176b2-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="176b2-129">Property</span></span>|<span data-ttu-id="176b2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="176b2-130">Type</span></span>|<span data-ttu-id="176b2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="176b2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="176b2-132">id</span><span class="sxs-lookup"><span data-stu-id="176b2-132">id</span></span>|<span data-ttu-id="176b2-133">String</span><span class="sxs-lookup"><span data-stu-id="176b2-133">String</span></span>|<span data-ttu-id="176b2-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="176b2-134">Key of the entity.</span></span>|
|<span data-ttu-id="176b2-135">**Integração**</span><span class="sxs-lookup"><span data-stu-id="176b2-135">**Onboarding**</span></span>|
|<span data-ttu-id="176b2-136">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="176b2-136">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="176b2-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="176b2-137">Boolean</span></span>|<span data-ttu-id="176b2-138">Se a conta está ativada para sincronizar aplicativos do Microsoft Store para Empresa.</span><span class="sxs-lookup"><span data-stu-id="176b2-138">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="176b2-139">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="176b2-139">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="176b2-140">String</span><span class="sxs-lookup"><span data-stu-id="176b2-140">String</span></span>|<span data-ttu-id="176b2-141">As informações sobre a localidade usada para sincronizar aplicativos do Microsoft Store para Empresas.</span><span class="sxs-lookup"><span data-stu-id="176b2-141">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="176b2-142">Culturas específicas de um país/região.</span><span class="sxs-lookup"><span data-stu-id="176b2-142">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="176b2-143">Os nomes dessas culturas seguem a RFC 4646 (Windows Vista e mais recentes).</span><span class="sxs-lookup"><span data-stu-id="176b2-143">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="176b2-144">O formato é <languagecode2>-<country/regioncode2>, onde <languagecode2> é um código em duas letras minúsculas derivado da ISO 639-1 e <country/regioncode2> é um código em duas letras maiúsculas derivado da ISO 3166.</span><span class="sxs-lookup"><span data-stu-id="176b2-144">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="176b2-145">Por exemplo, en-US para inglês (Estados Unidos) é uma cultura específica.</span><span class="sxs-lookup"><span data-stu-id="176b2-145">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="176b2-146">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="176b2-146">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="176b2-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="176b2-147">DateTimeOffset</span></span>|<span data-ttu-id="176b2-148">A última vez em uma sincronização de aplicativo na Microsoft Store para Empresas foi concluída.</span><span class="sxs-lookup"><span data-stu-id="176b2-148">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="176b2-149">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="176b2-149">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="176b2-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="176b2-150">DateTimeOffset</span></span>|<span data-ttu-id="176b2-151">A última vez que os aplicativos da Microsoft Store para Empresas foram sincronizados com êxito para essa conta.</span><span class="sxs-lookup"><span data-stu-id="176b2-151">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|

## <a name="response"></a><span data-ttu-id="176b2-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="176b2-152">Response</span></span>
<span data-ttu-id="176b2-153">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="176b2-153">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="176b2-154">Exemplo de solicitação</span><span class="sxs-lookup"><span data-stu-id="176b2-154">Example request</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

## <a name="example-response"></a><span data-ttu-id="176b2-155">Resposta de exemplo</span><span class="sxs-lookup"><span data-stu-id="176b2-155">Example response</span></span>

<span data-ttu-id="176b2-156">O objeto de resposta mostrado aqui pode estar truncado por brevidade.</span><span class="sxs-lookup"><span data-stu-id="176b2-156">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="176b2-157">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="176b2-157">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```



