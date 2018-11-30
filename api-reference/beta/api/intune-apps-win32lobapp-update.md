---
title: Atualizar win32LobApp
description: Atualize as propriedades de um objeto win32LobApp.
ms.openlocfilehash: ec543716bcbf387b9b880535702a832a25319302
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040265"
---
# <a name="update-win32lobapp"></a><span data-ttu-id="119de-103">Atualizar win32LobApp</span><span class="sxs-lookup"><span data-stu-id="119de-103">Update win32LobApp</span></span>

> <span data-ttu-id="119de-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="119de-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="119de-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="119de-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="119de-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="119de-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="119de-107">Atualize as propriedades de um objeto [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="119de-107">Update the properties of a [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="119de-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="119de-108">Prerequisites</span></span>
<span data-ttu-id="119de-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="119de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="119de-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="119de-111">Permission type</span></span>|<span data-ttu-id="119de-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="119de-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="119de-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="119de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="119de-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="119de-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="119de-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="119de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="119de-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="119de-116">Not supported.</span></span>|
|<span data-ttu-id="119de-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="119de-117">Application</span></span>|<span data-ttu-id="119de-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="119de-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="119de-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="119de-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="119de-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="119de-120">Request headers</span></span>
|<span data-ttu-id="119de-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="119de-121">Header</span></span>|<span data-ttu-id="119de-122">Valor</span><span class="sxs-lookup"><span data-stu-id="119de-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="119de-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="119de-123">Authorization</span></span>|<span data-ttu-id="119de-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="119de-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="119de-125">Accept</span><span class="sxs-lookup"><span data-stu-id="119de-125">Accept</span></span>|<span data-ttu-id="119de-126">application/json</span><span class="sxs-lookup"><span data-stu-id="119de-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="119de-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="119de-127">Request body</span></span>
<span data-ttu-id="119de-128">No corpo da solicitação, fornece uma representação JSON para o objeto [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="119de-128">In the request body, supply a JSON representation for the [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

<span data-ttu-id="119de-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [win32LobApp](../resources/intune-apps-win32lobapp.md).</span><span class="sxs-lookup"><span data-stu-id="119de-129">The following table shows the properties that are required when you create the [win32LobApp](../resources/intune-apps-win32lobapp.md).</span></span>

|<span data-ttu-id="119de-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="119de-130">Property</span></span>|<span data-ttu-id="119de-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="119de-131">Type</span></span>|<span data-ttu-id="119de-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="119de-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="119de-133">id</span><span class="sxs-lookup"><span data-stu-id="119de-133">id</span></span>|<span data-ttu-id="119de-134">String</span><span class="sxs-lookup"><span data-stu-id="119de-134">String</span></span>|<span data-ttu-id="119de-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="119de-135">Key of the entity.</span></span> <span data-ttu-id="119de-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="119de-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="119de-137">displayName</span><span class="sxs-lookup"><span data-stu-id="119de-137">displayName</span></span>|<span data-ttu-id="119de-138">String</span><span class="sxs-lookup"><span data-stu-id="119de-138">String</span></span>|<span data-ttu-id="119de-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="119de-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="119de-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="119de-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="119de-141">description</span><span class="sxs-lookup"><span data-stu-id="119de-141">description</span></span>|<span data-ttu-id="119de-142">String</span><span class="sxs-lookup"><span data-stu-id="119de-142">String</span></span>|<span data-ttu-id="119de-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="119de-143">The description of the app.</span></span> <span data-ttu-id="119de-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="119de-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="119de-145">publisher</span><span class="sxs-lookup"><span data-stu-id="119de-145">publisher</span></span>|<span data-ttu-id="119de-146">String</span><span class="sxs-lookup"><span data-stu-id="119de-146">String</span></span>|<span data-ttu-id="119de-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="119de-147">The publisher of the app.</span></span> <span data-ttu-id="119de-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="119de-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="119de-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="119de-149">largeIcon</span></span>|[<span data-ttu-id="119de-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="119de-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="119de-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="119de-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="119de-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="119de-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="119de-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="119de-153">createdDateTime</span></span>|<span data-ttu-id="119de-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="119de-154">DateTimeOffset</span></span>|<span data-ttu-id="119de-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="119de-155">The date and time the app was created.</span></span> <span data-ttu-id="119de-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="119de-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="119de-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="119de-157">lastModifiedDateTime</span></span>|<span data-ttu-id="119de-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="119de-158">DateTimeOffset</span></span>|<span data-ttu-id="119de-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="119de-159">The date and time the app was last modified.</span></span> <span data-ttu-id="119de-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="119de-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="119de-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="119de-161">isFeatured</span></span>|<span data-ttu-id="119de-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="119de-162">Boolean</span></span>|<span data-ttu-id="119de-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="119de-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="119de-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="119de-164">privacyInformationUrl</span></span>|<span data-ttu-id="119de-165">String</span><span class="sxs-lookup"><span data-stu-id="119de-165">String</span></span>|<span data-ttu-id="119de-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="119de-166">The privacy statement Url.</span></span> <span data-ttu-id="119de-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="119de-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="119de-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="119de-168">informationUrl</span></span>|<span data-ttu-id="119de-169">String</span><span class="sxs-lookup"><span data-stu-id="119de-169">String</span></span>|<span data-ttu-id="119de-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="119de-170">The more information Url.</span></span> <span data-ttu-id="119de-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="119de-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="119de-172">owner</span><span class="sxs-lookup"><span data-stu-id="119de-172">owner</span></span>|<span data-ttu-id="119de-173">String</span><span class="sxs-lookup"><span data-stu-id="119de-173">String</span></span>|<span data-ttu-id="119de-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="119de-174">The owner of the app.</span></span> <span data-ttu-id="119de-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="119de-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="119de-176">developer</span><span class="sxs-lookup"><span data-stu-id="119de-176">developer</span></span>|<span data-ttu-id="119de-177">String</span><span class="sxs-lookup"><span data-stu-id="119de-177">String</span></span>|<span data-ttu-id="119de-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="119de-178">The developer of the app.</span></span> <span data-ttu-id="119de-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="119de-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="119de-180">Observações</span><span class="sxs-lookup"><span data-stu-id="119de-180">notes</span></span>|<span data-ttu-id="119de-181">String</span><span class="sxs-lookup"><span data-stu-id="119de-181">String</span></span>|<span data-ttu-id="119de-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="119de-182">Notes for the app.</span></span> <span data-ttu-id="119de-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="119de-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="119de-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="119de-184">uploadState</span></span>|<span data-ttu-id="119de-185">Int32</span><span class="sxs-lookup"><span data-stu-id="119de-185">Int32</span></span>|<span data-ttu-id="119de-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="119de-186">The upload state.</span></span> <span data-ttu-id="119de-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="119de-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="119de-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="119de-188">publishingState</span></span>|[<span data-ttu-id="119de-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="119de-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="119de-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="119de-190">The publishing state for the app.</span></span> <span data-ttu-id="119de-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="119de-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="119de-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="119de-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="119de-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="119de-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="119de-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="119de-194">committedContentVersion</span></span>|<span data-ttu-id="119de-195">String</span><span class="sxs-lookup"><span data-stu-id="119de-195">String</span></span>|<span data-ttu-id="119de-196">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="119de-196">The internal committed content version.</span></span> <span data-ttu-id="119de-197">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="119de-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="119de-198">fileName</span><span class="sxs-lookup"><span data-stu-id="119de-198">fileName</span></span>|<span data-ttu-id="119de-199">String</span><span class="sxs-lookup"><span data-stu-id="119de-199">String</span></span>|<span data-ttu-id="119de-200">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="119de-200">The name of the main Lob application file.</span></span> <span data-ttu-id="119de-201">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="119de-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="119de-202">size</span><span class="sxs-lookup"><span data-stu-id="119de-202">size</span></span>|<span data-ttu-id="119de-203">Int64</span><span class="sxs-lookup"><span data-stu-id="119de-203">Int64</span></span>|<span data-ttu-id="119de-204">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="119de-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="119de-205">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="119de-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="119de-206">installCommandLine</span><span class="sxs-lookup"><span data-stu-id="119de-206">installCommandLine</span></span>|<span data-ttu-id="119de-207">String</span><span class="sxs-lookup"><span data-stu-id="119de-207">String</span></span>|<span data-ttu-id="119de-208">A linha de comando para instalar este aplicativo</span><span class="sxs-lookup"><span data-stu-id="119de-208">The command line to install this app</span></span>|
|<span data-ttu-id="119de-209">uninstallCommandLine</span><span class="sxs-lookup"><span data-stu-id="119de-209">uninstallCommandLine</span></span>|<span data-ttu-id="119de-210">String</span><span class="sxs-lookup"><span data-stu-id="119de-210">String</span></span>|<span data-ttu-id="119de-211">A linha de comando para desinstalar este aplicativo</span><span class="sxs-lookup"><span data-stu-id="119de-211">The command line to uninstall this app</span></span>|
|<span data-ttu-id="119de-212">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="119de-212">applicableArchitectures</span></span>|[<span data-ttu-id="119de-213">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="119de-213">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="119de-214">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="119de-214">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="119de-215">Os valores possíveis são: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="119de-215">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="119de-216">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="119de-216">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="119de-217">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="119de-217">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="119de-218">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="119de-218">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="119de-219">minimumFreeDiskSpaceInMB</span><span class="sxs-lookup"><span data-stu-id="119de-219">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="119de-220">Int32</span><span class="sxs-lookup"><span data-stu-id="119de-220">Int32</span></span>|<span data-ttu-id="119de-221">O valor para o espaço livre em disco mínimo que é necessário para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="119de-221">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="119de-222">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="119de-222">minimumMemoryInMB</span></span>|<span data-ttu-id="119de-223">Int32</span><span class="sxs-lookup"><span data-stu-id="119de-223">Int32</span></span>|<span data-ttu-id="119de-224">O valor para o mínimo de memória físico que é necessário para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="119de-224">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="119de-225">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="119de-225">minimumNumberOfProcessors</span></span>|<span data-ttu-id="119de-226">Int32</span><span class="sxs-lookup"><span data-stu-id="119de-226">Int32</span></span>|<span data-ttu-id="119de-227">O valor para o número mínimo de processadores, que é necessário para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="119de-227">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="119de-228">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="119de-228">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="119de-229">Int32</span><span class="sxs-lookup"><span data-stu-id="119de-229">Int32</span></span>|<span data-ttu-id="119de-230">O valor para a velocidade de CPU mínima, que é necessário para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="119de-230">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="119de-231">detectionRules</span><span class="sxs-lookup"><span data-stu-id="119de-231">detectionRules</span></span>|<span data-ttu-id="119de-232">coleção [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="119de-232">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="119de-233">As regras de detecção para detectar app Win32 linha de negócios (LoB).</span><span class="sxs-lookup"><span data-stu-id="119de-233">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="119de-234">installExperience</span><span class="sxs-lookup"><span data-stu-id="119de-234">installExperience</span></span>|[<span data-ttu-id="119de-235">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="119de-235">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="119de-236">A experiência da instalação para esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="119de-236">The install experience for this app.</span></span>|
|<span data-ttu-id="119de-237">returnCodes</span><span class="sxs-lookup"><span data-stu-id="119de-237">returnCodes</span></span>|<span data-ttu-id="119de-238">coleção [win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)</span><span class="sxs-lookup"><span data-stu-id="119de-238">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="119de-239">Os códigos de retorno para lançar o comportamento da instalação.</span><span class="sxs-lookup"><span data-stu-id="119de-239">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="119de-240">msiInformation</span><span class="sxs-lookup"><span data-stu-id="119de-240">msiInformation</span></span>|[<span data-ttu-id="119de-241">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="119de-241">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="119de-242">Os detalhes do MSI se este aplicativo Win32 é um aplicativo MSI.</span><span class="sxs-lookup"><span data-stu-id="119de-242">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="119de-243">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="119de-243">setupFilePath</span></span>|<span data-ttu-id="119de-244">String</span><span class="sxs-lookup"><span data-stu-id="119de-244">String</span></span>|<span data-ttu-id="119de-245">O caminho relativo do arquivo de instalação no pacote Win32LobApp criptografado.</span><span class="sxs-lookup"><span data-stu-id="119de-245">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|



## <a name="response"></a><span data-ttu-id="119de-246">Resposta</span><span class="sxs-lookup"><span data-stu-id="119de-246">Response</span></span>
<span data-ttu-id="119de-247">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [win32LobApp](../resources/intune-apps-win32lobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="119de-247">If successful, this method returns a `200 OK` response code and an updated [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="119de-248">Exemplo</span><span class="sxs-lookup"><span data-stu-id="119de-248">Example</span></span>
### <a name="request"></a><span data-ttu-id="119de-249">Solicitação</span><span class="sxs-lookup"><span data-stu-id="119de-249">Request</span></span>
<span data-ttu-id="119de-250">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="119de-250">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2214

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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser"
  },
  "setupFilePath": "Setup File Path value"
}
```

### <a name="response"></a><span data-ttu-id="119de-251">Resposta</span><span class="sxs-lookup"><span data-stu-id="119de-251">Response</span></span>
<span data-ttu-id="119de-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="119de-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2372

{
  "@odata.type": "#microsoft.graph.win32LobApp",
  "id": "9607b530-b530-9607-30b5-079630b50796",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser"
  },
  "setupFilePath": "Setup File Path value"
}
```





