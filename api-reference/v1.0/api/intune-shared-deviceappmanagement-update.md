---
title: Atualizar deviceAppManagement
description: Atualizar as propriedades de um objeto de deviceAppManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 419bdc52dd9dbc7b67528b4a8b109bb309547f95
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019193"
---
# <a name="update-deviceappmanagement"></a><span data-ttu-id="9ab00-103">Atualizar deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="9ab00-103">Update deviceAppManagement</span></span>

<span data-ttu-id="9ab00-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ab00-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9ab00-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9ab00-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ab00-106">Atualizar as propriedades de um objeto de [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="9ab00-106">Update the properties of a [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ab00-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9ab00-107">Prerequisites</span></span>
<span data-ttu-id="9ab00-108">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="9ab00-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="9ab00-109">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ab00-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="9ab00-110">Observe que a permissão adequada varia de acordo com o fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="9ab00-110">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="9ab00-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ab00-111">Permission type</span></span>|<span data-ttu-id="9ab00-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9ab00-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ab00-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ab00-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9ab00-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ab00-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9ab00-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ab00-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ab00-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ab00-116">Not supported.</span></span>|
|<span data-ttu-id="9ab00-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ab00-117">Application</span></span>|<span data-ttu-id="9ab00-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ab00-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ab00-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ab00-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="9ab00-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ab00-120">Request headers</span></span>
|<span data-ttu-id="9ab00-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9ab00-121">Header</span></span>|<span data-ttu-id="9ab00-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9ab00-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ab00-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ab00-123">Authorization</span></span>|<span data-ttu-id="9ab00-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ab00-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ab00-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9ab00-125">Accept</span></span>|<span data-ttu-id="9ab00-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9ab00-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ab00-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ab00-127">Request body</span></span>
<span data-ttu-id="9ab00-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="9ab00-128">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

<span data-ttu-id="9ab00-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="9ab00-129">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span></span>

|<span data-ttu-id="9ab00-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ab00-130">Property</span></span>|<span data-ttu-id="9ab00-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ab00-131">Type</span></span>|<span data-ttu-id="9ab00-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ab00-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ab00-133">id</span><span class="sxs-lookup"><span data-stu-id="9ab00-133">id</span></span>|<span data-ttu-id="9ab00-134">String</span><span class="sxs-lookup"><span data-stu-id="9ab00-134">String</span></span>|<span data-ttu-id="9ab00-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9ab00-135">Key of the entity.</span></span>|
|<span data-ttu-id="9ab00-136">**Integração**</span><span class="sxs-lookup"><span data-stu-id="9ab00-136">**Onboarding**</span></span>|
|<span data-ttu-id="9ab00-137">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="9ab00-137">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="9ab00-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ab00-138">Boolean</span></span>|<span data-ttu-id="9ab00-139">Se a conta está ativada para sincronizar aplicativos do Microsoft Store para Empresa.</span><span class="sxs-lookup"><span data-stu-id="9ab00-139">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="9ab00-140">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="9ab00-140">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="9ab00-141">String</span><span class="sxs-lookup"><span data-stu-id="9ab00-141">String</span></span>|<span data-ttu-id="9ab00-142">As informações sobre a localidade usada para sincronizar aplicativos do Microsoft Store para Empresas.</span><span class="sxs-lookup"><span data-stu-id="9ab00-142">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="9ab00-143">Culturas específicas de um país/região.</span><span class="sxs-lookup"><span data-stu-id="9ab00-143">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="9ab00-144">Os nomes dessas culturas seguem a RFC 4646 (Windows Vista e mais recentes).</span><span class="sxs-lookup"><span data-stu-id="9ab00-144">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="9ab00-145">O formato é <languagecode2>-<country/regioncode2>, onde <languagecode2> é um código em duas letras minúsculas derivado da ISO 639-1 e <country/regioncode2> é um código em duas letras maiúsculas derivado da ISO 3166.</span><span class="sxs-lookup"><span data-stu-id="9ab00-145">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="9ab00-146">Por exemplo, en-US para inglês (Estados Unidos) é uma cultura específica.</span><span class="sxs-lookup"><span data-stu-id="9ab00-146">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="9ab00-147">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="9ab00-147">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="9ab00-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ab00-148">DateTimeOffset</span></span>|<span data-ttu-id="9ab00-149">A última vez em uma sincronização de aplicativo na Microsoft Store para Empresas foi concluída.</span><span class="sxs-lookup"><span data-stu-id="9ab00-149">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="9ab00-150">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9ab00-150">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="9ab00-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ab00-151">DateTimeOffset</span></span>|<span data-ttu-id="9ab00-152">A última vez que os aplicativos da Microsoft Store para Empresas foram sincronizados com êxito para essa conta.</span><span class="sxs-lookup"><span data-stu-id="9ab00-152">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|

## <a name="response"></a><span data-ttu-id="9ab00-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ab00-153">Response</span></span>
<span data-ttu-id="9ab00-154">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ab00-154">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="9ab00-155">Exemplo de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ab00-155">Example request</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

## <a name="example-response"></a><span data-ttu-id="9ab00-156">Resposta de exemplo</span><span class="sxs-lookup"><span data-stu-id="9ab00-156">Example response</span></span>

<span data-ttu-id="9ab00-157">O objeto de resposta mostrado aqui pode estar truncado por brevidade.</span><span class="sxs-lookup"><span data-stu-id="9ab00-157">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9ab00-158">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ab00-158">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```









