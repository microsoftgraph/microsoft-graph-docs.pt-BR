---
title: Atualizar deviceAppManagement
description: Atualizar as propriedades de um objeto de deviceAppManagement.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6abcaec953c07e6974d3a421ff26612710d390b2
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940170"
---
# <a name="update-deviceappmanagement"></a><span data-ttu-id="427ab-103">Atualizar deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="427ab-103">Update deviceAppManagement</span></span>

> <span data-ttu-id="427ab-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="427ab-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="427ab-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="427ab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="427ab-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="427ab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="427ab-107">Atualizar as propriedades de um objeto de [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="427ab-107">Update the properties of a [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="427ab-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="427ab-108">Prerequisites</span></span>
<span data-ttu-id="427ab-109">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="427ab-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="427ab-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="427ab-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="427ab-111">Observe que a permissão adequada varia de acordo com o fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="427ab-111">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="427ab-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="427ab-112">Permission type</span></span>|<span data-ttu-id="427ab-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="427ab-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="427ab-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="427ab-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="427ab-115">&nbsp;&nbsp; **Aplicativos**, **livros**, \*\*\*\* integração, integração de **parceiros**ou conjunto de **políticas**</span><span class="sxs-lookup"><span data-stu-id="427ab-115">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, **Partner Integration**, or **Policy Set**</span></span> | <span data-ttu-id="427ab-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="427ab-116">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="427ab-117">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="427ab-117">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="427ab-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="427ab-118">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="427ab-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="427ab-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="427ab-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="427ab-120">Not supported.</span></span> |
| <span data-ttu-id="427ab-121">Application</span><span class="sxs-lookup"><span data-stu-id="427ab-121">Application</span></span> | |
| <span data-ttu-id="427ab-122">&nbsp;&nbsp; **Aplicativos**, **livros**, \*\*\*\* integração, integração de **parceiros**ou conjunto de **políticas**</span><span class="sxs-lookup"><span data-stu-id="427ab-122">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, **Partner Integration**, or **Policy Set**</span></span> | <span data-ttu-id="427ab-123">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="427ab-123">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="427ab-124">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="427ab-124">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="427ab-125">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="427ab-125">DeviceManagementManagedDevices.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="427ab-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="427ab-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="427ab-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="427ab-127">Request headers</span></span>
|<span data-ttu-id="427ab-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="427ab-128">Header</span></span>|<span data-ttu-id="427ab-129">Valor</span><span class="sxs-lookup"><span data-stu-id="427ab-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="427ab-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="427ab-130">Authorization</span></span>|<span data-ttu-id="427ab-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="427ab-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="427ab-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="427ab-132">Accept</span></span>|<span data-ttu-id="427ab-133">application/json</span><span class="sxs-lookup"><span data-stu-id="427ab-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="427ab-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="427ab-134">Request body</span></span>
<span data-ttu-id="427ab-135">No corpo da solicitação, forneça uma representação JSON do objeto [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="427ab-135">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

<span data-ttu-id="427ab-136">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="427ab-136">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span></span>

|<span data-ttu-id="427ab-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="427ab-137">Property</span></span>|<span data-ttu-id="427ab-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="427ab-138">Type</span></span>|<span data-ttu-id="427ab-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="427ab-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="427ab-140">id</span><span class="sxs-lookup"><span data-stu-id="427ab-140">id</span></span>|<span data-ttu-id="427ab-141">String</span><span class="sxs-lookup"><span data-stu-id="427ab-141">String</span></span>|<span data-ttu-id="427ab-142">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="427ab-142">Key of the entity.</span></span>|
|<span data-ttu-id="427ab-143">**Integração**</span><span class="sxs-lookup"><span data-stu-id="427ab-143">**On-boarding**</span></span>|
|<span data-ttu-id="427ab-144">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="427ab-144">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="427ab-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="427ab-145">Boolean</span></span>|<span data-ttu-id="427ab-146">Se a conta está ativada para sincronizar aplicativos do Microsoft Store para Empresa.</span><span class="sxs-lookup"><span data-stu-id="427ab-146">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="427ab-147">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="427ab-147">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="427ab-148">String</span><span class="sxs-lookup"><span data-stu-id="427ab-148">String</span></span>|<span data-ttu-id="427ab-149">As informações sobre a localidade usada para sincronizar aplicativos do Microsoft Store para Empresas.</span><span class="sxs-lookup"><span data-stu-id="427ab-149">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="427ab-150">Culturas específicas de um país/região.</span><span class="sxs-lookup"><span data-stu-id="427ab-150">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="427ab-151">Os nomes dessas culturas seguem a RFC 4646 (Windows Vista e mais recentes).</span><span class="sxs-lookup"><span data-stu-id="427ab-151">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="427ab-152">O formato é <languagecode2>-<country/regioncode2>, onde <languagecode2> é um código em duas letras minúsculas derivado da ISO 639-1 e <country/regioncode2> é um código em duas letras maiúsculas derivado da ISO 3166.</span><span class="sxs-lookup"><span data-stu-id="427ab-152">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="427ab-153">Por exemplo, en-US para inglês (Estados Unidos) é uma cultura específica.</span><span class="sxs-lookup"><span data-stu-id="427ab-153">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="427ab-154">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="427ab-154">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="427ab-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="427ab-155">DateTimeOffset</span></span>|<span data-ttu-id="427ab-156">A última vez em uma sincronização de aplicativo na Microsoft Store para Empresas foi concluída.</span><span class="sxs-lookup"><span data-stu-id="427ab-156">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="427ab-157">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="427ab-157">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="427ab-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="427ab-158">DateTimeOffset</span></span>|<span data-ttu-id="427ab-159">A última vez que os aplicativos da Microsoft Store para Empresas foram sincronizados com êxito para essa conta.</span><span class="sxs-lookup"><span data-stu-id="427ab-159">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|
|<span data-ttu-id="427ab-160">microsoftStoreForBusinessPortalSelection</span><span class="sxs-lookup"><span data-stu-id="427ab-160">microsoftStoreForBusinessPortalSelection</span></span>|[<span data-ttu-id="427ab-161">microsoftStoreForBusinessPortalSelectionOptions</span><span class="sxs-lookup"><span data-stu-id="427ab-161">microsoftStoreForBusinessPortalSelectionOptions</span></span>](../resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)|<span data-ttu-id="427ab-162">As informações do portal do usuário final são usadas para sincronizar aplicativos da Microsoft Store para empresas com o portal da empresa do Intune.</span><span class="sxs-lookup"><span data-stu-id="427ab-162">The end user portal information is used to sync applications from the Microsoft Store for Business to Intune Company Portal.</span></span> <span data-ttu-id="427ab-163">Há três opções a serem escolhidas \[em "somente portal da empresa", "portal da empresa e repositório privado", "somente\]repositório privado".</span><span class="sxs-lookup"><span data-stu-id="427ab-163">There are three options to pick from \['Company portal only', 'Company portal and private store', 'Private store only'\].</span></span> <span data-ttu-id="427ab-164">Os valores possíveis são: `none`, `companyPortal`, `privateStore`.</span><span class="sxs-lookup"><span data-stu-id="427ab-164">Possible values are: `none`, `companyPortal`, `privateStore`.</span></span>|

<span data-ttu-id="427ab-165">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="427ab-165">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="427ab-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="427ab-166">Response</span></span>
<span data-ttu-id="427ab-167">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="427ab-167">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="427ab-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="427ab-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="427ab-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="427ab-169">Request</span></span>

<span data-ttu-id="427ab-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="427ab-170">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="427ab-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="427ab-171">Response</span></span>

<span data-ttu-id="427ab-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="427ab-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```











