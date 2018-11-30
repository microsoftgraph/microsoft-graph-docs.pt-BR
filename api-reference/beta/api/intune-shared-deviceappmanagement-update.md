---
title: Atualizar deviceAppManagement
description: Atualizar as propriedades de um objeto de deviceAppManagement.
ms.openlocfilehash: e842e81f098a42e064be1aa00616a84d7f08eb34
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038332"
---
# <a name="update-deviceappmanagement"></a><span data-ttu-id="911d2-103">Atualizar deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="911d2-103">Update deviceAppManagement</span></span>

> <span data-ttu-id="911d2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="911d2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="911d2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="911d2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="911d2-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="911d2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="911d2-107">Atualizar as propriedades de um objeto de [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="911d2-107">Update the properties of a [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="911d2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="911d2-108">Prerequisites</span></span>
<span data-ttu-id="911d2-109">Uma das seguintes permissões é necessário chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="911d2-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="911d2-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="911d2-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="911d2-111">Observe que a permissão apropriada varia de acordo com o fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="911d2-111">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="911d2-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="911d2-112">Permission type</span></span>|<span data-ttu-id="911d2-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="911d2-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="911d2-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="911d2-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="911d2-115">&nbsp;&nbsp; **Apps**, **livros**ou **inclusão**</span><span class="sxs-lookup"><span data-stu-id="911d2-115">&nbsp; &nbsp; **Apps**, **books**, or **onboarding**</span></span> | <span data-ttu-id="911d2-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="911d2-116">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="911d2-117">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="911d2-117">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="911d2-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="911d2-118">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="911d2-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="911d2-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="911d2-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="911d2-120">Not supported.</span></span> |
| <span data-ttu-id="911d2-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="911d2-121">Application</span></span> | <span data-ttu-id="911d2-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="911d2-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="911d2-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="911d2-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="911d2-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="911d2-124">Request headers</span></span>
|<span data-ttu-id="911d2-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="911d2-125">Header</span></span>|<span data-ttu-id="911d2-126">Valor</span><span class="sxs-lookup"><span data-stu-id="911d2-126">Value</span></span>|
|:---|:---|
|<span data-ttu-id="911d2-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="911d2-127">Authorization</span></span>|<span data-ttu-id="911d2-128">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="911d2-128">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="911d2-129">Accept</span><span class="sxs-lookup"><span data-stu-id="911d2-129">Accept</span></span>|<span data-ttu-id="911d2-130">application/json</span><span class="sxs-lookup"><span data-stu-id="911d2-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="911d2-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="911d2-131">Request body</span></span>
<span data-ttu-id="911d2-132">No corpo da solicitação, forneça uma representação JSON do objeto [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="911d2-132">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

<span data-ttu-id="911d2-133">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="911d2-133">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span></span>

|<span data-ttu-id="911d2-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="911d2-134">Property</span></span>|<span data-ttu-id="911d2-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="911d2-135">Type</span></span>|<span data-ttu-id="911d2-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="911d2-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="911d2-137">id</span><span class="sxs-lookup"><span data-stu-id="911d2-137">id</span></span>|<span data-ttu-id="911d2-138">String</span><span class="sxs-lookup"><span data-stu-id="911d2-138">String</span></span>|<span data-ttu-id="911d2-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="911d2-139">Key of the entity.</span></span>|
|<span data-ttu-id="911d2-140">**Nível de contratação**</span><span class="sxs-lookup"><span data-stu-id="911d2-140">**On-boarding**</span></span>|
|<span data-ttu-id="911d2-141">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="911d2-141">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="911d2-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="911d2-142">Boolean</span></span>|<span data-ttu-id="911d2-143">Se a conta está ativada para sincronizar aplicativos do Microsoft Store para Empresa.</span><span class="sxs-lookup"><span data-stu-id="911d2-143">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="911d2-144">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="911d2-144">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="911d2-145">String</span><span class="sxs-lookup"><span data-stu-id="911d2-145">String</span></span>|<span data-ttu-id="911d2-146">As informações sobre a localidade usada para sincronizar aplicativos do Microsoft Store para Empresas.</span><span class="sxs-lookup"><span data-stu-id="911d2-146">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="911d2-147">Culturas específicas de um país/região.</span><span class="sxs-lookup"><span data-stu-id="911d2-147">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="911d2-148">Os nomes dessas culturas seguem a RFC 4646 (Windows Vista e mais recentes).</span><span class="sxs-lookup"><span data-stu-id="911d2-148">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="911d2-149">O formato é <languagecode2>-<country/regioncode2>, onde <languagecode2> é um código em duas letras minúsculas derivado da ISO 639-1 e <country/regioncode2> é um código em duas letras maiúsculas derivado da ISO 3166.</span><span class="sxs-lookup"><span data-stu-id="911d2-149">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="911d2-150">Por exemplo, en-US para inglês (Estados Unidos) é uma cultura específica.</span><span class="sxs-lookup"><span data-stu-id="911d2-150">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="911d2-151">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="911d2-151">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="911d2-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="911d2-152">DateTimeOffset</span></span>|<span data-ttu-id="911d2-153">A última vez em uma sincronização de aplicativo na Microsoft Store para Empresas foi concluída.</span><span class="sxs-lookup"><span data-stu-id="911d2-153">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="911d2-154">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="911d2-154">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="911d2-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="911d2-155">DateTimeOffset</span></span>|<span data-ttu-id="911d2-156">A última vez que os aplicativos da Microsoft Store para Empresas foram sincronizados com êxito para essa conta.</span><span class="sxs-lookup"><span data-stu-id="911d2-156">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|
|<span data-ttu-id="911d2-157">microsoftStoreForBusinessPortalSelection</span><span class="sxs-lookup"><span data-stu-id="911d2-157">microsoftStoreForBusinessPortalSelection</span></span>|[<span data-ttu-id="911d2-158">microsoftStoreForBusinessPortalSelectionOptions</span><span class="sxs-lookup"><span data-stu-id="911d2-158">microsoftStoreForBusinessPortalSelectionOptions</span></span>](../resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)|<span data-ttu-id="911d2-159">As informações do portal de usuário final são usadas para sincronizar os aplicativos do Microsoft Store for Business para Intune Portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="911d2-159">The end user portal information is used to sync applications from the Microsoft Store for Business to Intune Company Portal.</span></span> <span data-ttu-id="911d2-160">Existem três opções para selecionar \['Somente para portal da empresa', 'Empresa portal e particular armazenar', 'Somente armazenamento particular'\].</span><span class="sxs-lookup"><span data-stu-id="911d2-160">There are three options to pick from \['Company portal only', 'Company portal and private store', 'Private store only'\].</span></span> <span data-ttu-id="911d2-161">Os valores possíveis são: `none`, `companyPortal`, `privateStore`.</span><span class="sxs-lookup"><span data-stu-id="911d2-161">Possible values are: `none`, `companyPortal`, `privateStore`.</span></span>|

<span data-ttu-id="911d2-162">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="911d2-162">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="911d2-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="911d2-163">Response</span></span>
<span data-ttu-id="911d2-164">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="911d2-164">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="911d2-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="911d2-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="911d2-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="911d2-166">Request</span></span>

<span data-ttu-id="911d2-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="911d2-167">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="911d2-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="911d2-168">Response</span></span>

<span data-ttu-id="911d2-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="911d2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```



