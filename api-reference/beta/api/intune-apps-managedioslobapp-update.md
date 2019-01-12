---
title: Atualizar managedIOSLobApp
description: Atualiza as propriedades de um objeto managedIOSLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 82a3a3b1b9e767e0fe8cb93b6c2380896ae22851
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939963"
---
# <a name="update-managedioslobapp"></a><span data-ttu-id="51168-103">Atualizar managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="51168-103">Update managedIOSLobApp</span></span>

> <span data-ttu-id="51168-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="51168-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51168-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="51168-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="51168-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="51168-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51168-107">Atualiza as propriedades de um objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="51168-107">Update the properties of a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="51168-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="51168-108">Prerequisites</span></span>
<span data-ttu-id="51168-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51168-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51168-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51168-111">Permission type</span></span>|<span data-ttu-id="51168-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="51168-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51168-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51168-113">Delegated (work or school account)</span></span>|<span data-ttu-id="51168-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51168-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="51168-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51168-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51168-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51168-116">Not supported.</span></span>|
|<span data-ttu-id="51168-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51168-117">Application</span></span>|<span data-ttu-id="51168-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51168-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51168-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51168-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="51168-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51168-120">Request headers</span></span>
|<span data-ttu-id="51168-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="51168-121">Header</span></span>|<span data-ttu-id="51168-122">Valor</span><span class="sxs-lookup"><span data-stu-id="51168-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51168-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="51168-123">Authorization</span></span>|<span data-ttu-id="51168-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51168-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51168-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="51168-125">Accept</span></span>|<span data-ttu-id="51168-126">application/json</span><span class="sxs-lookup"><span data-stu-id="51168-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51168-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51168-127">Request body</span></span>
<span data-ttu-id="51168-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="51168-128">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

<span data-ttu-id="51168-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="51168-129">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span></span>

|<span data-ttu-id="51168-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51168-130">Property</span></span>|<span data-ttu-id="51168-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="51168-131">Type</span></span>|<span data-ttu-id="51168-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="51168-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51168-133">id</span><span class="sxs-lookup"><span data-stu-id="51168-133">id</span></span>|<span data-ttu-id="51168-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51168-134">String</span></span>|<span data-ttu-id="51168-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="51168-135">Key of the entity.</span></span> <span data-ttu-id="51168-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51168-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51168-137">displayName</span><span class="sxs-lookup"><span data-stu-id="51168-137">displayName</span></span>|<span data-ttu-id="51168-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51168-138">String</span></span>|<span data-ttu-id="51168-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="51168-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="51168-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51168-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51168-141">description</span><span class="sxs-lookup"><span data-stu-id="51168-141">description</span></span>|<span data-ttu-id="51168-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51168-142">String</span></span>|<span data-ttu-id="51168-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="51168-143">The description of the app.</span></span> <span data-ttu-id="51168-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51168-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51168-145">publisher</span><span class="sxs-lookup"><span data-stu-id="51168-145">publisher</span></span>|<span data-ttu-id="51168-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51168-146">String</span></span>|<span data-ttu-id="51168-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="51168-147">The publisher of the app.</span></span> <span data-ttu-id="51168-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51168-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51168-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="51168-149">largeIcon</span></span>|[<span data-ttu-id="51168-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="51168-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="51168-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="51168-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="51168-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51168-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51168-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="51168-153">createdDateTime</span></span>|<span data-ttu-id="51168-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51168-154">DateTimeOffset</span></span>|<span data-ttu-id="51168-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="51168-155">The date and time the app was created.</span></span> <span data-ttu-id="51168-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51168-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51168-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="51168-157">lastModifiedDateTime</span></span>|<span data-ttu-id="51168-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51168-158">DateTimeOffset</span></span>|<span data-ttu-id="51168-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="51168-159">The date and time the app was last modified.</span></span> <span data-ttu-id="51168-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51168-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51168-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="51168-161">isFeatured</span></span>|<span data-ttu-id="51168-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="51168-162">Boolean</span></span>|<span data-ttu-id="51168-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51168-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51168-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="51168-164">privacyInformationUrl</span></span>|<span data-ttu-id="51168-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51168-165">String</span></span>|<span data-ttu-id="51168-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="51168-166">The privacy statement Url.</span></span> <span data-ttu-id="51168-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51168-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51168-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="51168-168">informationUrl</span></span>|<span data-ttu-id="51168-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51168-169">String</span></span>|<span data-ttu-id="51168-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="51168-170">The more information Url.</span></span> <span data-ttu-id="51168-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51168-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51168-172">owner</span><span class="sxs-lookup"><span data-stu-id="51168-172">owner</span></span>|<span data-ttu-id="51168-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51168-173">String</span></span>|<span data-ttu-id="51168-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="51168-174">The owner of the app.</span></span> <span data-ttu-id="51168-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51168-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51168-176">developer</span><span class="sxs-lookup"><span data-stu-id="51168-176">developer</span></span>|<span data-ttu-id="51168-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51168-177">String</span></span>|<span data-ttu-id="51168-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="51168-178">The developer of the app.</span></span> <span data-ttu-id="51168-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51168-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51168-180">Observações</span><span class="sxs-lookup"><span data-stu-id="51168-180">notes</span></span>|<span data-ttu-id="51168-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51168-181">String</span></span>|<span data-ttu-id="51168-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="51168-182">Notes for the app.</span></span> <span data-ttu-id="51168-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51168-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51168-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="51168-184">uploadState</span></span>|<span data-ttu-id="51168-185">Int32</span><span class="sxs-lookup"><span data-stu-id="51168-185">Int32</span></span>|<span data-ttu-id="51168-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="51168-186">The upload state.</span></span> <span data-ttu-id="51168-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="51168-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51168-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="51168-188">publishingState</span></span>|[<span data-ttu-id="51168-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="51168-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="51168-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="51168-190">The publishing state for the app.</span></span> <span data-ttu-id="51168-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="51168-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="51168-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="51168-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="51168-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="51168-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="51168-194">appAvailability</span><span class="sxs-lookup"><span data-stu-id="51168-194">appAvailability</span></span>|[<span data-ttu-id="51168-195">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="51168-195">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="51168-196">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="51168-196">The Application's availability.</span></span> <span data-ttu-id="51168-197">Herdada do [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="51168-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="51168-198">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="51168-198">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="51168-199">version</span><span class="sxs-lookup"><span data-stu-id="51168-199">version</span></span>|<span data-ttu-id="51168-200">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51168-200">String</span></span>|<span data-ttu-id="51168-201">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="51168-201">The Application's version.</span></span> <span data-ttu-id="51168-202">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="51168-202">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="51168-203">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="51168-203">committedContentVersion</span></span>|<span data-ttu-id="51168-204">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51168-204">String</span></span>|<span data-ttu-id="51168-205">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="51168-205">The internal committed content version.</span></span> <span data-ttu-id="51168-206">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="51168-206">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="51168-207">fileName</span><span class="sxs-lookup"><span data-stu-id="51168-207">fileName</span></span>|<span data-ttu-id="51168-208">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51168-208">String</span></span>|<span data-ttu-id="51168-209">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="51168-209">The name of the main Lob application file.</span></span> <span data-ttu-id="51168-210">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="51168-210">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="51168-211">size</span><span class="sxs-lookup"><span data-stu-id="51168-211">size</span></span>|<span data-ttu-id="51168-212">Int64</span><span class="sxs-lookup"><span data-stu-id="51168-212">Int64</span></span>|<span data-ttu-id="51168-213">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="51168-213">The total size, including all uploaded files.</span></span> <span data-ttu-id="51168-214">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="51168-214">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="51168-215">bundleId</span><span class="sxs-lookup"><span data-stu-id="51168-215">bundleId</span></span>|<span data-ttu-id="51168-216">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51168-216">String</span></span>|<span data-ttu-id="51168-217">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="51168-217">The Identity Name.</span></span>|
|<span data-ttu-id="51168-218">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="51168-218">applicableDeviceType</span></span>|[<span data-ttu-id="51168-219">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="51168-219">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="51168-220">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="51168-220">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="51168-221">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="51168-221">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="51168-222">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="51168-222">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="51168-223">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="51168-223">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="51168-224">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="51168-224">expirationDateTime</span></span>|<span data-ttu-id="51168-225">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51168-225">DateTimeOffset</span></span>|<span data-ttu-id="51168-226">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="51168-226">The expiration time.</span></span>|
|<span data-ttu-id="51168-227">versionNumber</span><span class="sxs-lookup"><span data-stu-id="51168-227">versionNumber</span></span>|<span data-ttu-id="51168-228">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51168-228">String</span></span>|<span data-ttu-id="51168-229">O número de versão do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="51168-229">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="51168-230">buildNumber</span><span class="sxs-lookup"><span data-stu-id="51168-230">buildNumber</span></span>|<span data-ttu-id="51168-231">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51168-231">String</span></span>|<span data-ttu-id="51168-232">O número de build do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="51168-232">The build number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="51168-233">identityVersion</span><span class="sxs-lookup"><span data-stu-id="51168-233">identityVersion</span></span>|<span data-ttu-id="51168-234">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51168-234">String</span></span>|<span data-ttu-id="51168-235">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="51168-235">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="51168-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="51168-236">Response</span></span>
<span data-ttu-id="51168-237">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51168-237">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51168-238">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51168-238">Example</span></span>
### <a name="request"></a><span data-ttu-id="51168-239">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51168-239">Request</span></span>
<span data-ttu-id="51168-240">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="51168-240">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="51168-241">Resposta</span><span class="sxs-lookup"><span data-stu-id="51168-241">Response</span></span>
<span data-ttu-id="51168-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51168-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





