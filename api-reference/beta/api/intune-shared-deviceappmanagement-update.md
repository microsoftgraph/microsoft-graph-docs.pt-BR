---
title: Atualizar deviceAppManagement
description: Atualizar as propriedades de um objeto de deviceAppManagement.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e03b6936d17297159115193a287bc96999c83d71
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458928"
---
# <a name="update-deviceappmanagement"></a><span data-ttu-id="ff13b-103">Atualizar deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="ff13b-103">Update deviceAppManagement</span></span>

<span data-ttu-id="ff13b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ff13b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff13b-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ff13b-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ff13b-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ff13b-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff13b-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ff13b-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff13b-108">Atualizar as propriedades de um objeto de [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="ff13b-108">Update the properties of a [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ff13b-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ff13b-109">Prerequisites</span></span>
<span data-ttu-id="ff13b-110">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="ff13b-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="ff13b-111">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff13b-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="ff13b-112">Observe que a permissão adequada varia de acordo com o fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="ff13b-112">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="ff13b-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff13b-113">Permission type</span></span>|<span data-ttu-id="ff13b-114">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ff13b-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="ff13b-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff13b-115">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="ff13b-116">&nbsp;&nbsp; **Aplicativos**, **livros**, \*\*\*\* integração, integração de **parceiros**ou conjunto de **políticas**</span><span class="sxs-lookup"><span data-stu-id="ff13b-116">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, **Partner Integration**, or **Policy Set**</span></span> | <span data-ttu-id="ff13b-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff13b-117">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="ff13b-118">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="ff13b-118">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="ff13b-119">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff13b-119">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="ff13b-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff13b-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff13b-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff13b-121">Not supported.</span></span> |
| <span data-ttu-id="ff13b-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff13b-122">Application</span></span> | |
| <span data-ttu-id="ff13b-123">&nbsp;&nbsp; **Aplicativos**, **livros**, \*\*\*\* integração, integração de **parceiros**ou conjunto de **políticas**</span><span class="sxs-lookup"><span data-stu-id="ff13b-123">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, **Partner Integration**, or **Policy Set**</span></span> | <span data-ttu-id="ff13b-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff13b-124">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="ff13b-125">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="ff13b-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="ff13b-126">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff13b-126">DeviceManagementManagedDevices.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff13b-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff13b-127">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="ff13b-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff13b-128">Request headers</span></span>
|<span data-ttu-id="ff13b-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ff13b-129">Header</span></span>|<span data-ttu-id="ff13b-130">Valor</span><span class="sxs-lookup"><span data-stu-id="ff13b-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff13b-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff13b-131">Authorization</span></span>|<span data-ttu-id="ff13b-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff13b-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff13b-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ff13b-133">Accept</span></span>|<span data-ttu-id="ff13b-134">application/json</span><span class="sxs-lookup"><span data-stu-id="ff13b-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff13b-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff13b-135">Request body</span></span>
<span data-ttu-id="ff13b-136">No corpo da solicitação, forneça uma representação JSON do objeto [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="ff13b-136">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

<span data-ttu-id="ff13b-137">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="ff13b-137">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span></span>

|<span data-ttu-id="ff13b-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff13b-138">Property</span></span>|<span data-ttu-id="ff13b-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff13b-139">Type</span></span>|<span data-ttu-id="ff13b-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff13b-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff13b-141">id</span><span class="sxs-lookup"><span data-stu-id="ff13b-141">id</span></span>|<span data-ttu-id="ff13b-142">String</span><span class="sxs-lookup"><span data-stu-id="ff13b-142">String</span></span>|<span data-ttu-id="ff13b-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ff13b-143">Key of the entity.</span></span>|
|<span data-ttu-id="ff13b-144">**Integração**</span><span class="sxs-lookup"><span data-stu-id="ff13b-144">**On-boarding**</span></span>|
|<span data-ttu-id="ff13b-145">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="ff13b-145">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="ff13b-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff13b-146">Boolean</span></span>|<span data-ttu-id="ff13b-147">Se a conta está ativada para sincronizar aplicativos do Microsoft Store para Empresa.</span><span class="sxs-lookup"><span data-stu-id="ff13b-147">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="ff13b-148">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="ff13b-148">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="ff13b-149">String</span><span class="sxs-lookup"><span data-stu-id="ff13b-149">String</span></span>|<span data-ttu-id="ff13b-150">As informações sobre a localidade usada para sincronizar aplicativos do Microsoft Store para Empresas.</span><span class="sxs-lookup"><span data-stu-id="ff13b-150">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="ff13b-151">Culturas específicas de um país/região.</span><span class="sxs-lookup"><span data-stu-id="ff13b-151">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="ff13b-152">Os nomes dessas culturas seguem a RFC 4646 (Windows Vista e mais recentes).</span><span class="sxs-lookup"><span data-stu-id="ff13b-152">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="ff13b-153">O formato é <languagecode2>-<country/regioncode2>, onde <languagecode2> é um código em duas letras minúsculas derivado da ISO 639-1 e <country/regioncode2> é um código em duas letras maiúsculas derivado da ISO 3166.</span><span class="sxs-lookup"><span data-stu-id="ff13b-153">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="ff13b-154">Por exemplo, en-US para inglês (Estados Unidos) é uma cultura específica.</span><span class="sxs-lookup"><span data-stu-id="ff13b-154">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="ff13b-155">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="ff13b-155">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="ff13b-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff13b-156">DateTimeOffset</span></span>|<span data-ttu-id="ff13b-157">A última vez em uma sincronização de aplicativo na Microsoft Store para Empresas foi concluída.</span><span class="sxs-lookup"><span data-stu-id="ff13b-157">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="ff13b-158">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ff13b-158">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="ff13b-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff13b-159">DateTimeOffset</span></span>|<span data-ttu-id="ff13b-160">A última vez que os aplicativos da Microsoft Store para Empresas foram sincronizados com êxito para essa conta.</span><span class="sxs-lookup"><span data-stu-id="ff13b-160">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|
|<span data-ttu-id="ff13b-161">microsoftStoreForBusinessPortalSelection</span><span class="sxs-lookup"><span data-stu-id="ff13b-161">microsoftStoreForBusinessPortalSelection</span></span>|[<span data-ttu-id="ff13b-162">microsoftStoreForBusinessPortalSelectionOptions</span><span class="sxs-lookup"><span data-stu-id="ff13b-162">microsoftStoreForBusinessPortalSelectionOptions</span></span>](../resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)|<span data-ttu-id="ff13b-163">As informações do portal do usuário final são usadas para sincronizar aplicativos da Microsoft Store para empresas com o portal da empresa do Intune.</span><span class="sxs-lookup"><span data-stu-id="ff13b-163">The end user portal information is used to sync applications from the Microsoft Store for Business to Intune Company Portal.</span></span> <span data-ttu-id="ff13b-164">Há três opções a serem escolhidas \[em "somente portal da empresa", "portal da empresa e repositório privado", "somente\]repositório privado".</span><span class="sxs-lookup"><span data-stu-id="ff13b-164">There are three options to pick from \['Company portal only', 'Company portal and private store', 'Private store only'\].</span></span> <span data-ttu-id="ff13b-165">Os valores possíveis são: `none`, `companyPortal`, `privateStore`.</span><span class="sxs-lookup"><span data-stu-id="ff13b-165">Possible values are: `none`, `companyPortal`, `privateStore`.</span></span>|

<span data-ttu-id="ff13b-166">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ff13b-166">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="ff13b-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff13b-167">Response</span></span>
<span data-ttu-id="ff13b-168">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff13b-168">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff13b-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff13b-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff13b-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff13b-170">Request</span></span>

<span data-ttu-id="ff13b-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff13b-171">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="ff13b-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff13b-172">Response</span></span>

<span data-ttu-id="ff13b-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff13b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```











