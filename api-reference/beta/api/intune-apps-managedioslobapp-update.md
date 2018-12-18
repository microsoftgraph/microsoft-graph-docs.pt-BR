---
title: Atualizar managedIOSLobApp
description: Atualiza as propriedades de um objeto managedIOSLobApp.
author: tfitzmac
ms.openlocfilehash: af73dac3e1ccb785664f48a02837cec369b91297
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325505"
---
# <a name="update-managedioslobapp"></a><span data-ttu-id="12f93-103">Atualizar managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="12f93-103">Update managedIOSLobApp</span></span>

> <span data-ttu-id="12f93-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="12f93-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12f93-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="12f93-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="12f93-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="12f93-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12f93-107">Atualiza as propriedades de um objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="12f93-107">Update the properties of a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="12f93-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="12f93-108">Prerequisites</span></span>
<span data-ttu-id="12f93-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12f93-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12f93-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12f93-111">Permission type</span></span>|<span data-ttu-id="12f93-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="12f93-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12f93-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12f93-113">Delegated (work or school account)</span></span>|<span data-ttu-id="12f93-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12f93-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="12f93-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12f93-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12f93-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12f93-116">Not supported.</span></span>|
|<span data-ttu-id="12f93-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12f93-117">Application</span></span>|<span data-ttu-id="12f93-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12f93-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12f93-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12f93-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="12f93-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12f93-120">Request headers</span></span>
|<span data-ttu-id="12f93-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="12f93-121">Header</span></span>|<span data-ttu-id="12f93-122">Valor</span><span class="sxs-lookup"><span data-stu-id="12f93-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12f93-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="12f93-123">Authorization</span></span>|<span data-ttu-id="12f93-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12f93-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12f93-125">Accept</span><span class="sxs-lookup"><span data-stu-id="12f93-125">Accept</span></span>|<span data-ttu-id="12f93-126">application/json</span><span class="sxs-lookup"><span data-stu-id="12f93-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12f93-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12f93-127">Request body</span></span>
<span data-ttu-id="12f93-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="12f93-128">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

<span data-ttu-id="12f93-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="12f93-129">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span></span>

|<span data-ttu-id="12f93-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12f93-130">Property</span></span>|<span data-ttu-id="12f93-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="12f93-131">Type</span></span>|<span data-ttu-id="12f93-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="12f93-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12f93-133">id</span><span class="sxs-lookup"><span data-stu-id="12f93-133">id</span></span>|<span data-ttu-id="12f93-134">String</span><span class="sxs-lookup"><span data-stu-id="12f93-134">String</span></span>|<span data-ttu-id="12f93-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="12f93-135">Key of the entity.</span></span> <span data-ttu-id="12f93-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12f93-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="12f93-137">displayName</span><span class="sxs-lookup"><span data-stu-id="12f93-137">displayName</span></span>|<span data-ttu-id="12f93-138">String</span><span class="sxs-lookup"><span data-stu-id="12f93-138">String</span></span>|<span data-ttu-id="12f93-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="12f93-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="12f93-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12f93-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="12f93-141">description</span><span class="sxs-lookup"><span data-stu-id="12f93-141">description</span></span>|<span data-ttu-id="12f93-142">String</span><span class="sxs-lookup"><span data-stu-id="12f93-142">String</span></span>|<span data-ttu-id="12f93-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="12f93-143">The description of the app.</span></span> <span data-ttu-id="12f93-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12f93-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="12f93-145">publisher</span><span class="sxs-lookup"><span data-stu-id="12f93-145">publisher</span></span>|<span data-ttu-id="12f93-146">String</span><span class="sxs-lookup"><span data-stu-id="12f93-146">String</span></span>|<span data-ttu-id="12f93-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="12f93-147">The publisher of the app.</span></span> <span data-ttu-id="12f93-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12f93-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="12f93-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="12f93-149">largeIcon</span></span>|[<span data-ttu-id="12f93-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="12f93-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="12f93-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="12f93-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="12f93-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12f93-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="12f93-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="12f93-153">createdDateTime</span></span>|<span data-ttu-id="12f93-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12f93-154">DateTimeOffset</span></span>|<span data-ttu-id="12f93-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="12f93-155">The date and time the app was created.</span></span> <span data-ttu-id="12f93-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12f93-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="12f93-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="12f93-157">lastModifiedDateTime</span></span>|<span data-ttu-id="12f93-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12f93-158">DateTimeOffset</span></span>|<span data-ttu-id="12f93-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="12f93-159">The date and time the app was last modified.</span></span> <span data-ttu-id="12f93-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12f93-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="12f93-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="12f93-161">isFeatured</span></span>|<span data-ttu-id="12f93-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="12f93-162">Boolean</span></span>|<span data-ttu-id="12f93-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12f93-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="12f93-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="12f93-164">privacyInformationUrl</span></span>|<span data-ttu-id="12f93-165">String</span><span class="sxs-lookup"><span data-stu-id="12f93-165">String</span></span>|<span data-ttu-id="12f93-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="12f93-166">The privacy statement Url.</span></span> <span data-ttu-id="12f93-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12f93-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="12f93-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="12f93-168">informationUrl</span></span>|<span data-ttu-id="12f93-169">String</span><span class="sxs-lookup"><span data-stu-id="12f93-169">String</span></span>|<span data-ttu-id="12f93-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="12f93-170">The more information Url.</span></span> <span data-ttu-id="12f93-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12f93-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="12f93-172">owner</span><span class="sxs-lookup"><span data-stu-id="12f93-172">owner</span></span>|<span data-ttu-id="12f93-173">String</span><span class="sxs-lookup"><span data-stu-id="12f93-173">String</span></span>|<span data-ttu-id="12f93-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="12f93-174">The owner of the app.</span></span> <span data-ttu-id="12f93-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12f93-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="12f93-176">developer</span><span class="sxs-lookup"><span data-stu-id="12f93-176">developer</span></span>|<span data-ttu-id="12f93-177">String</span><span class="sxs-lookup"><span data-stu-id="12f93-177">String</span></span>|<span data-ttu-id="12f93-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="12f93-178">The developer of the app.</span></span> <span data-ttu-id="12f93-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12f93-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="12f93-180">Observações</span><span class="sxs-lookup"><span data-stu-id="12f93-180">notes</span></span>|<span data-ttu-id="12f93-181">String</span><span class="sxs-lookup"><span data-stu-id="12f93-181">String</span></span>|<span data-ttu-id="12f93-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="12f93-182">Notes for the app.</span></span> <span data-ttu-id="12f93-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12f93-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="12f93-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="12f93-184">uploadState</span></span>|<span data-ttu-id="12f93-185">Int32</span><span class="sxs-lookup"><span data-stu-id="12f93-185">Int32</span></span>|<span data-ttu-id="12f93-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="12f93-186">The upload state.</span></span> <span data-ttu-id="12f93-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12f93-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="12f93-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="12f93-188">publishingState</span></span>|[<span data-ttu-id="12f93-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="12f93-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="12f93-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="12f93-190">The publishing state for the app.</span></span> <span data-ttu-id="12f93-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="12f93-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="12f93-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="12f93-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="12f93-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="12f93-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="12f93-194">appAvailability</span><span class="sxs-lookup"><span data-stu-id="12f93-194">appAvailability</span></span>|[<span data-ttu-id="12f93-195">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="12f93-195">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="12f93-196">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="12f93-196">The Application's availability.</span></span> <span data-ttu-id="12f93-197">Herdada do [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="12f93-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="12f93-198">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="12f93-198">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="12f93-199">version</span><span class="sxs-lookup"><span data-stu-id="12f93-199">version</span></span>|<span data-ttu-id="12f93-200">String</span><span class="sxs-lookup"><span data-stu-id="12f93-200">String</span></span>|<span data-ttu-id="12f93-201">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="12f93-201">The Application's version.</span></span> <span data-ttu-id="12f93-202">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="12f93-202">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="12f93-203">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="12f93-203">committedContentVersion</span></span>|<span data-ttu-id="12f93-204">String</span><span class="sxs-lookup"><span data-stu-id="12f93-204">String</span></span>|<span data-ttu-id="12f93-205">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="12f93-205">The internal committed content version.</span></span> <span data-ttu-id="12f93-206">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="12f93-206">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="12f93-207">fileName</span><span class="sxs-lookup"><span data-stu-id="12f93-207">fileName</span></span>|<span data-ttu-id="12f93-208">String</span><span class="sxs-lookup"><span data-stu-id="12f93-208">String</span></span>|<span data-ttu-id="12f93-209">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="12f93-209">The name of the main Lob application file.</span></span> <span data-ttu-id="12f93-210">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="12f93-210">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="12f93-211">size</span><span class="sxs-lookup"><span data-stu-id="12f93-211">size</span></span>|<span data-ttu-id="12f93-212">Int64</span><span class="sxs-lookup"><span data-stu-id="12f93-212">Int64</span></span>|<span data-ttu-id="12f93-213">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="12f93-213">The total size, including all uploaded files.</span></span> <span data-ttu-id="12f93-214">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="12f93-214">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="12f93-215">bundleId</span><span class="sxs-lookup"><span data-stu-id="12f93-215">bundleId</span></span>|<span data-ttu-id="12f93-216">String</span><span class="sxs-lookup"><span data-stu-id="12f93-216">String</span></span>|<span data-ttu-id="12f93-217">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="12f93-217">The Identity Name.</span></span>|
|<span data-ttu-id="12f93-218">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="12f93-218">applicableDeviceType</span></span>|[<span data-ttu-id="12f93-219">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="12f93-219">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="12f93-220">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="12f93-220">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="12f93-221">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="12f93-221">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="12f93-222">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="12f93-222">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="12f93-223">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="12f93-223">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="12f93-224">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="12f93-224">expirationDateTime</span></span>|<span data-ttu-id="12f93-225">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12f93-225">DateTimeOffset</span></span>|<span data-ttu-id="12f93-226">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="12f93-226">The expiration time.</span></span>|
|<span data-ttu-id="12f93-227">versionNumber</span><span class="sxs-lookup"><span data-stu-id="12f93-227">versionNumber</span></span>|<span data-ttu-id="12f93-228">String</span><span class="sxs-lookup"><span data-stu-id="12f93-228">String</span></span>|<span data-ttu-id="12f93-229">O número de versão do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="12f93-229">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="12f93-230">buildNumber</span><span class="sxs-lookup"><span data-stu-id="12f93-230">buildNumber</span></span>|<span data-ttu-id="12f93-231">String</span><span class="sxs-lookup"><span data-stu-id="12f93-231">String</span></span>|<span data-ttu-id="12f93-232">O número de build do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="12f93-232">The build number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="12f93-233">identityVersion</span><span class="sxs-lookup"><span data-stu-id="12f93-233">identityVersion</span></span>|<span data-ttu-id="12f93-234">String</span><span class="sxs-lookup"><span data-stu-id="12f93-234">String</span></span>|<span data-ttu-id="12f93-235">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="12f93-235">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="12f93-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="12f93-236">Response</span></span>
<span data-ttu-id="12f93-237">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12f93-237">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12f93-238">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12f93-238">Example</span></span>
### <a name="request"></a><span data-ttu-id="12f93-239">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12f93-239">Request</span></span>
<span data-ttu-id="12f93-240">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="12f93-240">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1366

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="12f93-241">Resposta</span><span class="sxs-lookup"><span data-stu-id="12f93-241">Response</span></span>
<span data-ttu-id="12f93-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="12f93-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1529

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```





