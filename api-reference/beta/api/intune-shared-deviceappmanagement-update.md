---
title: Atualizar deviceAppManagement
description: Atualizar as propriedades de um objeto de deviceAppManagement.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bed5a7fd19afb736bdbd5e11eece9dbbd7c3424c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801254"
---
# <a name="update-deviceappmanagement"></a><span data-ttu-id="8880a-103">Atualizar deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="8880a-103">Update deviceAppManagement</span></span>

> <span data-ttu-id="8880a-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8880a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8880a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8880a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8880a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8880a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8880a-107">Atualizar as propriedades de um objeto de [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="8880a-107">Update the properties of a [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8880a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8880a-108">Prerequisites</span></span>
<span data-ttu-id="8880a-109">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="8880a-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="8880a-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8880a-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="8880a-111">Observe que a permissão adequada varia de acordo com o fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="8880a-111">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="8880a-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8880a-112">Permission type</span></span>|<span data-ttu-id="8880a-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8880a-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="8880a-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8880a-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="8880a-115">&nbsp;&nbsp; **Aplicativos**, **livros**, **onboarding**integração, integração de **parceiros**ou conjunto de **políticas**</span><span class="sxs-lookup"><span data-stu-id="8880a-115">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, **Partner Integration**, or **Policy Set**</span></span> | <span data-ttu-id="8880a-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8880a-116">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="8880a-117">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="8880a-117">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="8880a-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8880a-118">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="8880a-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8880a-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8880a-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8880a-120">Not supported.</span></span> |
| <span data-ttu-id="8880a-121">Application</span><span class="sxs-lookup"><span data-stu-id="8880a-121">Application</span></span> | |
| <span data-ttu-id="8880a-122">&nbsp;&nbsp; **Aplicativos**, **livros**, **onboarding**integração, integração de **parceiros**ou conjunto de **políticas**</span><span class="sxs-lookup"><span data-stu-id="8880a-122">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, **Partner Integration**, or **Policy Set**</span></span> | <span data-ttu-id="8880a-123">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8880a-123">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="8880a-124">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="8880a-124">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="8880a-125">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8880a-125">DeviceManagementManagedDevices.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8880a-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8880a-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="8880a-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8880a-127">Request headers</span></span>
|<span data-ttu-id="8880a-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8880a-128">Header</span></span>|<span data-ttu-id="8880a-129">Valor</span><span class="sxs-lookup"><span data-stu-id="8880a-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8880a-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="8880a-130">Authorization</span></span>|<span data-ttu-id="8880a-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8880a-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8880a-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8880a-132">Accept</span></span>|<span data-ttu-id="8880a-133">application/json</span><span class="sxs-lookup"><span data-stu-id="8880a-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8880a-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8880a-134">Request body</span></span>
<span data-ttu-id="8880a-135">No corpo da solicitação, forneça uma representação JSON do objeto [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="8880a-135">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

<span data-ttu-id="8880a-136">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="8880a-136">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span></span>

|<span data-ttu-id="8880a-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8880a-137">Property</span></span>|<span data-ttu-id="8880a-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="8880a-138">Type</span></span>|<span data-ttu-id="8880a-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="8880a-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8880a-140">id</span><span class="sxs-lookup"><span data-stu-id="8880a-140">id</span></span>|<span data-ttu-id="8880a-141">String</span><span class="sxs-lookup"><span data-stu-id="8880a-141">String</span></span>|<span data-ttu-id="8880a-142">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8880a-142">Key of the entity.</span></span>|
|<span data-ttu-id="8880a-143">**Integração**</span><span class="sxs-lookup"><span data-stu-id="8880a-143">**On-boarding**</span></span>|
|<span data-ttu-id="8880a-144">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="8880a-144">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="8880a-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="8880a-145">Boolean</span></span>|<span data-ttu-id="8880a-146">Se a conta está ativada para sincronizar aplicativos do Microsoft Store para Empresa.</span><span class="sxs-lookup"><span data-stu-id="8880a-146">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="8880a-147">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="8880a-147">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="8880a-148">String</span><span class="sxs-lookup"><span data-stu-id="8880a-148">String</span></span>|<span data-ttu-id="8880a-149">As informações sobre a localidade usada para sincronizar aplicativos do Microsoft Store para Empresas.</span><span class="sxs-lookup"><span data-stu-id="8880a-149">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="8880a-150">Culturas específicas de um país/região.</span><span class="sxs-lookup"><span data-stu-id="8880a-150">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="8880a-151">Os nomes dessas culturas seguem a RFC 4646 (Windows Vista e mais recentes).</span><span class="sxs-lookup"><span data-stu-id="8880a-151">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="8880a-152">O formato é <languagecode2>-<country/regioncode2>, onde <languagecode2> é um código em duas letras minúsculas derivado da ISO 639-1 e <country/regioncode2> é um código em duas letras maiúsculas derivado da ISO 3166.</span><span class="sxs-lookup"><span data-stu-id="8880a-152">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="8880a-153">Por exemplo, en-US para inglês (Estados Unidos) é uma cultura específica.</span><span class="sxs-lookup"><span data-stu-id="8880a-153">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="8880a-154">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="8880a-154">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="8880a-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8880a-155">DateTimeOffset</span></span>|<span data-ttu-id="8880a-156">A última vez em uma sincronização de aplicativo na Microsoft Store para Empresas foi concluída.</span><span class="sxs-lookup"><span data-stu-id="8880a-156">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="8880a-157">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="8880a-157">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="8880a-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8880a-158">DateTimeOffset</span></span>|<span data-ttu-id="8880a-159">A última vez que os aplicativos da Microsoft Store para Empresas foram sincronizados com êxito para essa conta.</span><span class="sxs-lookup"><span data-stu-id="8880a-159">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|
|<span data-ttu-id="8880a-160">microsoftStoreForBusinessPortalSelection</span><span class="sxs-lookup"><span data-stu-id="8880a-160">microsoftStoreForBusinessPortalSelection</span></span>|[<span data-ttu-id="8880a-161">microsoftStoreForBusinessPortalSelectionOptions</span><span class="sxs-lookup"><span data-stu-id="8880a-161">microsoftStoreForBusinessPortalSelectionOptions</span></span>](../resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)|<span data-ttu-id="8880a-162">As informações do portal do usuário final são usadas para sincronizar aplicativos da Microsoft Store para empresas com o portal da empresa do Intune.</span><span class="sxs-lookup"><span data-stu-id="8880a-162">The end user portal information is used to sync applications from the Microsoft Store for Business to Intune Company Portal.</span></span> <span data-ttu-id="8880a-163">Há três opções a serem escolhidas \[em "somente portal da empresa", "portal da empresa e repositório privado", "somente\]repositório privado".</span><span class="sxs-lookup"><span data-stu-id="8880a-163">There are three options to pick from \['Company portal only', 'Company portal and private store', 'Private store only'\].</span></span> <span data-ttu-id="8880a-164">Os valores possíveis são: `none`, `companyPortal`, `privateStore`.</span><span class="sxs-lookup"><span data-stu-id="8880a-164">Possible values are: `none`, `companyPortal`, `privateStore`.</span></span>|

<span data-ttu-id="8880a-165">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8880a-165">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="8880a-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="8880a-166">Response</span></span>
<span data-ttu-id="8880a-167">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8880a-167">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8880a-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8880a-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="8880a-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8880a-169">Request</span></span>

<span data-ttu-id="8880a-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8880a-170">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="8880a-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="8880a-171">Response</span></span>

<span data-ttu-id="8880a-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8880a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```










