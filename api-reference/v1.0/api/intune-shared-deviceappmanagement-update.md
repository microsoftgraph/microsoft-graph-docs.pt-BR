---
title: Atualizar deviceAppManagement
description: Atualizar as propriedades de um objeto de deviceAppManagement.
ms.openlocfilehash: 92d792f0ee4bab4923eda03cd488ece0a75f8ab3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006527"
---
# <a name="update-deviceappmanagement"></a><span data-ttu-id="fe416-103">Atualizar deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="fe416-103">Update deviceAppManagement</span></span>

> <span data-ttu-id="fe416-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fe416-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fe416-105">Atualizar as propriedades de um objeto de [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="fe416-105">Update the properties of a [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fe416-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fe416-106">Prerequisites</span></span>
<span data-ttu-id="fe416-107">Uma das seguintes permissões é necessário chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="fe416-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="fe416-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe416-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="fe416-109">Observe que a permissão apropriada varia de acordo com o fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="fe416-109">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="fe416-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe416-110">Permission type</span></span>|<span data-ttu-id="fe416-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fe416-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe416-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe416-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fe416-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe416-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fe416-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe416-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe416-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe416-115">Not supported.</span></span>|
|<span data-ttu-id="fe416-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe416-116">Application</span></span>|<span data-ttu-id="fe416-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe416-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe416-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe416-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="fe416-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe416-119">Request headers</span></span>
|<span data-ttu-id="fe416-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fe416-120">Header</span></span>|<span data-ttu-id="fe416-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fe416-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe416-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe416-122">Authorization</span></span>|<span data-ttu-id="fe416-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe416-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe416-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fe416-124">Accept</span></span>|<span data-ttu-id="fe416-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fe416-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe416-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe416-126">Request body</span></span>
<span data-ttu-id="fe416-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="fe416-127">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

<span data-ttu-id="fe416-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="fe416-128">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span></span>

|<span data-ttu-id="fe416-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe416-129">Property</span></span>|<span data-ttu-id="fe416-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe416-130">Type</span></span>|<span data-ttu-id="fe416-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe416-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe416-132">id</span><span class="sxs-lookup"><span data-stu-id="fe416-132">id</span></span>|<span data-ttu-id="fe416-133">String</span><span class="sxs-lookup"><span data-stu-id="fe416-133">String</span></span>|<span data-ttu-id="fe416-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fe416-134">Key of the entity.</span></span>|
|<span data-ttu-id="fe416-135">**Inclusão**</span><span class="sxs-lookup"><span data-stu-id="fe416-135">**Onboarding**</span></span>|
|<span data-ttu-id="fe416-136">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="fe416-136">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="fe416-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="fe416-137">Boolean</span></span>|<span data-ttu-id="fe416-138">Se a conta está ativada para sincronizar aplicativos do Microsoft Store para Empresa.</span><span class="sxs-lookup"><span data-stu-id="fe416-138">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="fe416-139">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="fe416-139">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="fe416-140">String</span><span class="sxs-lookup"><span data-stu-id="fe416-140">String</span></span>|<span data-ttu-id="fe416-141">As informações sobre a localidade usada para sincronizar aplicativos do Microsoft Store para Empresas.</span><span class="sxs-lookup"><span data-stu-id="fe416-141">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="fe416-142">Culturas específicas de um país/região.</span><span class="sxs-lookup"><span data-stu-id="fe416-142">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="fe416-143">Os nomes dessas culturas seguem a RFC 4646 (Windows Vista e mais recentes).</span><span class="sxs-lookup"><span data-stu-id="fe416-143">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="fe416-144">O formato é <languagecode2>-<country/regioncode2>, onde <languagecode2> é um código em duas letras minúsculas derivado da ISO 639-1 e <country/regioncode2> é um código em duas letras maiúsculas derivado da ISO 3166.</span><span class="sxs-lookup"><span data-stu-id="fe416-144">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="fe416-145">Por exemplo, en-US para inglês (Estados Unidos) é uma cultura específica.</span><span class="sxs-lookup"><span data-stu-id="fe416-145">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="fe416-146">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="fe416-146">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="fe416-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe416-147">DateTimeOffset</span></span>|<span data-ttu-id="fe416-148">A última vez em uma sincronização de aplicativo na Microsoft Store para Empresas foi concluída.</span><span class="sxs-lookup"><span data-stu-id="fe416-148">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="fe416-149">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="fe416-149">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="fe416-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe416-150">DateTimeOffset</span></span>|<span data-ttu-id="fe416-151">A última vez que os aplicativos da Microsoft Store para Empresas foram sincronizados com êxito para essa conta.</span><span class="sxs-lookup"><span data-stu-id="fe416-151">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|

## <a name="response"></a><span data-ttu-id="fe416-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe416-152">Response</span></span>
<span data-ttu-id="fe416-153">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe416-153">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="fe416-154">Exemplo de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe416-154">Example request</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

## <a name="example-response"></a><span data-ttu-id="fe416-155">Resposta de exemplo</span><span class="sxs-lookup"><span data-stu-id="fe416-155">Example response</span></span>

<span data-ttu-id="fe416-156">No objeto response mostrado aqui pode estar truncado para fins de concisão.</span><span class="sxs-lookup"><span data-stu-id="fe416-156">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fe416-157">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fe416-157">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```



