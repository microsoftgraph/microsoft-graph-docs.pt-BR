---
title: Atualizar iosLobApp
description: Atualiza as propriedades de um objeto iosLobApp.
author: tfitzmac
ms.openlocfilehash: f224064bdde083416e25de9675c150e6ce7ca226
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330279"
---
# <a name="update-ioslobapp"></a><span data-ttu-id="06379-103">Atualizar iosLobApp</span><span class="sxs-lookup"><span data-stu-id="06379-103">Update iosLobApp</span></span>

> <span data-ttu-id="06379-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="06379-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06379-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="06379-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06379-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="06379-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06379-107">Atualiza as propriedades de um objeto [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="06379-107">Update the properties of a [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="06379-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="06379-108">Prerequisites</span></span>
<span data-ttu-id="06379-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06379-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06379-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06379-111">Permission type</span></span>|<span data-ttu-id="06379-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="06379-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06379-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06379-113">Delegated (work or school account)</span></span>|<span data-ttu-id="06379-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06379-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="06379-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06379-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06379-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06379-116">Not supported.</span></span>|
|<span data-ttu-id="06379-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06379-117">Application</span></span>|<span data-ttu-id="06379-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06379-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06379-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06379-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="06379-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06379-120">Request headers</span></span>
|<span data-ttu-id="06379-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="06379-121">Header</span></span>|<span data-ttu-id="06379-122">Valor</span><span class="sxs-lookup"><span data-stu-id="06379-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06379-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="06379-123">Authorization</span></span>|<span data-ttu-id="06379-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06379-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06379-125">Accept</span><span class="sxs-lookup"><span data-stu-id="06379-125">Accept</span></span>|<span data-ttu-id="06379-126">application/json</span><span class="sxs-lookup"><span data-stu-id="06379-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06379-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06379-127">Request body</span></span>
<span data-ttu-id="06379-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="06379-128">In the request body, supply a JSON representation for the [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

<span data-ttu-id="06379-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosLobApp.](../resources/intune-apps-ioslobapp.md)</span><span class="sxs-lookup"><span data-stu-id="06379-129">The following table shows the properties that are required when you create the [iosLobApp](../resources/intune-apps-ioslobapp.md).</span></span>

|<span data-ttu-id="06379-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06379-130">Property</span></span>|<span data-ttu-id="06379-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="06379-131">Type</span></span>|<span data-ttu-id="06379-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="06379-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06379-133">id</span><span class="sxs-lookup"><span data-stu-id="06379-133">id</span></span>|<span data-ttu-id="06379-134">String</span><span class="sxs-lookup"><span data-stu-id="06379-134">String</span></span>|<span data-ttu-id="06379-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="06379-135">Key of the entity.</span></span> <span data-ttu-id="06379-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06379-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06379-137">displayName</span><span class="sxs-lookup"><span data-stu-id="06379-137">displayName</span></span>|<span data-ttu-id="06379-138">String</span><span class="sxs-lookup"><span data-stu-id="06379-138">String</span></span>|<span data-ttu-id="06379-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="06379-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="06379-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06379-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06379-141">description</span><span class="sxs-lookup"><span data-stu-id="06379-141">description</span></span>|<span data-ttu-id="06379-142">String</span><span class="sxs-lookup"><span data-stu-id="06379-142">String</span></span>|<span data-ttu-id="06379-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="06379-143">The description of the app.</span></span> <span data-ttu-id="06379-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06379-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06379-145">publisher</span><span class="sxs-lookup"><span data-stu-id="06379-145">publisher</span></span>|<span data-ttu-id="06379-146">String</span><span class="sxs-lookup"><span data-stu-id="06379-146">String</span></span>|<span data-ttu-id="06379-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="06379-147">The publisher of the app.</span></span> <span data-ttu-id="06379-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06379-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06379-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="06379-149">largeIcon</span></span>|[<span data-ttu-id="06379-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="06379-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="06379-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="06379-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="06379-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06379-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06379-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="06379-153">createdDateTime</span></span>|<span data-ttu-id="06379-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06379-154">DateTimeOffset</span></span>|<span data-ttu-id="06379-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="06379-155">The date and time the app was created.</span></span> <span data-ttu-id="06379-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06379-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06379-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06379-157">lastModifiedDateTime</span></span>|<span data-ttu-id="06379-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06379-158">DateTimeOffset</span></span>|<span data-ttu-id="06379-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="06379-159">The date and time the app was last modified.</span></span> <span data-ttu-id="06379-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06379-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06379-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="06379-161">isFeatured</span></span>|<span data-ttu-id="06379-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="06379-162">Boolean</span></span>|<span data-ttu-id="06379-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06379-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06379-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="06379-164">privacyInformationUrl</span></span>|<span data-ttu-id="06379-165">String</span><span class="sxs-lookup"><span data-stu-id="06379-165">String</span></span>|<span data-ttu-id="06379-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="06379-166">The privacy statement Url.</span></span> <span data-ttu-id="06379-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06379-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06379-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="06379-168">informationUrl</span></span>|<span data-ttu-id="06379-169">String</span><span class="sxs-lookup"><span data-stu-id="06379-169">String</span></span>|<span data-ttu-id="06379-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="06379-170">The more information Url.</span></span> <span data-ttu-id="06379-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06379-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06379-172">owner</span><span class="sxs-lookup"><span data-stu-id="06379-172">owner</span></span>|<span data-ttu-id="06379-173">String</span><span class="sxs-lookup"><span data-stu-id="06379-173">String</span></span>|<span data-ttu-id="06379-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="06379-174">The owner of the app.</span></span> <span data-ttu-id="06379-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06379-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06379-176">developer</span><span class="sxs-lookup"><span data-stu-id="06379-176">developer</span></span>|<span data-ttu-id="06379-177">String</span><span class="sxs-lookup"><span data-stu-id="06379-177">String</span></span>|<span data-ttu-id="06379-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="06379-178">The developer of the app.</span></span> <span data-ttu-id="06379-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06379-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06379-180">Observações</span><span class="sxs-lookup"><span data-stu-id="06379-180">notes</span></span>|<span data-ttu-id="06379-181">String</span><span class="sxs-lookup"><span data-stu-id="06379-181">String</span></span>|<span data-ttu-id="06379-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="06379-182">Notes for the app.</span></span> <span data-ttu-id="06379-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06379-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06379-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="06379-184">uploadState</span></span>|<span data-ttu-id="06379-185">Int32</span><span class="sxs-lookup"><span data-stu-id="06379-185">Int32</span></span>|<span data-ttu-id="06379-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="06379-186">The upload state.</span></span> <span data-ttu-id="06379-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06379-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06379-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="06379-188">publishingState</span></span>|[<span data-ttu-id="06379-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="06379-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="06379-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="06379-190">The publishing state for the app.</span></span> <span data-ttu-id="06379-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="06379-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="06379-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="06379-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="06379-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="06379-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="06379-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="06379-194">committedContentVersion</span></span>|<span data-ttu-id="06379-195">String</span><span class="sxs-lookup"><span data-stu-id="06379-195">String</span></span>|<span data-ttu-id="06379-196">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="06379-196">The internal committed content version.</span></span> <span data-ttu-id="06379-197">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="06379-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="06379-198">fileName</span><span class="sxs-lookup"><span data-stu-id="06379-198">fileName</span></span>|<span data-ttu-id="06379-199">String</span><span class="sxs-lookup"><span data-stu-id="06379-199">String</span></span>|<span data-ttu-id="06379-200">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="06379-200">The name of the main Lob application file.</span></span> <span data-ttu-id="06379-201">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="06379-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="06379-202">size</span><span class="sxs-lookup"><span data-stu-id="06379-202">size</span></span>|<span data-ttu-id="06379-203">Int64</span><span class="sxs-lookup"><span data-stu-id="06379-203">Int64</span></span>|<span data-ttu-id="06379-204">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="06379-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="06379-205">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="06379-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="06379-206">bundleId</span><span class="sxs-lookup"><span data-stu-id="06379-206">bundleId</span></span>|<span data-ttu-id="06379-207">String</span><span class="sxs-lookup"><span data-stu-id="06379-207">String</span></span>|<span data-ttu-id="06379-208">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="06379-208">The Identity Name.</span></span>|
|<span data-ttu-id="06379-209">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="06379-209">applicableDeviceType</span></span>|[<span data-ttu-id="06379-210">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="06379-210">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="06379-211">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="06379-211">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="06379-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="06379-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="06379-213">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="06379-213">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="06379-214">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="06379-214">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="06379-215">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="06379-215">expirationDateTime</span></span>|<span data-ttu-id="06379-216">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06379-216">DateTimeOffset</span></span>|<span data-ttu-id="06379-217">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="06379-217">The expiration time.</span></span>|
|<span data-ttu-id="06379-218">versionNumber</span><span class="sxs-lookup"><span data-stu-id="06379-218">versionNumber</span></span>|<span data-ttu-id="06379-219">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06379-219">String</span></span>|<span data-ttu-id="06379-220">O número de versão do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="06379-220">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="06379-221">buildNumber</span><span class="sxs-lookup"><span data-stu-id="06379-221">buildNumber</span></span>|<span data-ttu-id="06379-222">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06379-222">String</span></span>|<span data-ttu-id="06379-223">O número de build do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="06379-223">The build number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="06379-224">identityVersion</span><span class="sxs-lookup"><span data-stu-id="06379-224">identityVersion</span></span>|<span data-ttu-id="06379-225">String</span><span class="sxs-lookup"><span data-stu-id="06379-225">String</span></span>|<span data-ttu-id="06379-226">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="06379-226">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="06379-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="06379-227">Response</span></span>
<span data-ttu-id="06379-228">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [iosLobApp](../resources/intune-apps-ioslobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06379-228">If successful, this method returns a `200 OK` response code and an updated [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06379-229">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06379-229">Example</span></span>
### <a name="request"></a><span data-ttu-id="06379-230">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06379-230">Request</span></span>
<span data-ttu-id="06379-231">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06379-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1295

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

### <a name="response"></a><span data-ttu-id="06379-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="06379-232">Response</span></span>
<span data-ttu-id="06379-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06379-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1451

{
  "@odata.type": "#microsoft.graph.iosLobApp",
  "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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





