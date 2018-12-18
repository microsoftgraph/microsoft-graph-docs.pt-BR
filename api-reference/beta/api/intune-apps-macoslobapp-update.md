---
title: Atualizar macOSLobApp
description: Atualize as propriedades de um objeto macOSLobApp.
author: tfitzmac
ms.openlocfilehash: 0e465f84c930362f1607f434388e0c5c108c177f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303635"
---
# <a name="update-macoslobapp"></a><span data-ttu-id="d28b4-103">Atualizar macOSLobApp</span><span class="sxs-lookup"><span data-stu-id="d28b4-103">Update macOSLobApp</span></span>

> <span data-ttu-id="d28b4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d28b4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d28b4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d28b4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d28b4-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d28b4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d28b4-107">Atualize as propriedades de um objeto [macOSLobApp](../resources/intune-apps-macoslobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="d28b4-107">Update the properties of a [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d28b4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d28b4-108">Prerequisites</span></span>
<span data-ttu-id="d28b4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d28b4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d28b4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d28b4-111">Permission type</span></span>|<span data-ttu-id="d28b4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d28b4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d28b4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d28b4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d28b4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d28b4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d28b4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d28b4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d28b4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d28b4-116">Not supported.</span></span>|
|<span data-ttu-id="d28b4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d28b4-117">Application</span></span>|<span data-ttu-id="d28b4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d28b4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d28b4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d28b4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="d28b4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d28b4-120">Request headers</span></span>
|<span data-ttu-id="d28b4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d28b4-121">Header</span></span>|<span data-ttu-id="d28b4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d28b4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d28b4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d28b4-123">Authorization</span></span>|<span data-ttu-id="d28b4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d28b4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d28b4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d28b4-125">Accept</span></span>|<span data-ttu-id="d28b4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d28b4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d28b4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d28b4-127">Request body</span></span>
<span data-ttu-id="d28b4-128">No corpo da solicitação, fornece uma representação JSON para o objeto [macOSLobApp](../resources/intune-apps-macoslobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="d28b4-128">In the request body, supply a JSON representation for the [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

<span data-ttu-id="d28b4-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [macOSLobApp](../resources/intune-apps-macoslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="d28b4-129">The following table shows the properties that are required when you create the [macOSLobApp](../resources/intune-apps-macoslobapp.md).</span></span>

|<span data-ttu-id="d28b4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d28b4-130">Property</span></span>|<span data-ttu-id="d28b4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d28b4-131">Type</span></span>|<span data-ttu-id="d28b4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d28b4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d28b4-133">id</span><span class="sxs-lookup"><span data-stu-id="d28b4-133">id</span></span>|<span data-ttu-id="d28b4-134">String</span><span class="sxs-lookup"><span data-stu-id="d28b4-134">String</span></span>|<span data-ttu-id="d28b4-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d28b4-135">Key of the entity.</span></span> <span data-ttu-id="d28b4-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d28b4-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d28b4-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d28b4-137">displayName</span></span>|<span data-ttu-id="d28b4-138">String</span><span class="sxs-lookup"><span data-stu-id="d28b4-138">String</span></span>|<span data-ttu-id="d28b4-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="d28b4-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d28b4-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d28b4-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d28b4-141">description</span><span class="sxs-lookup"><span data-stu-id="d28b4-141">description</span></span>|<span data-ttu-id="d28b4-142">String</span><span class="sxs-lookup"><span data-stu-id="d28b4-142">String</span></span>|<span data-ttu-id="d28b4-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d28b4-143">The description of the app.</span></span> <span data-ttu-id="d28b4-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d28b4-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d28b4-145">publisher</span><span class="sxs-lookup"><span data-stu-id="d28b4-145">publisher</span></span>|<span data-ttu-id="d28b4-146">String</span><span class="sxs-lookup"><span data-stu-id="d28b4-146">String</span></span>|<span data-ttu-id="d28b4-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d28b4-147">The publisher of the app.</span></span> <span data-ttu-id="d28b4-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d28b4-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d28b4-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d28b4-149">largeIcon</span></span>|[<span data-ttu-id="d28b4-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d28b4-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d28b4-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="d28b4-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d28b4-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d28b4-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d28b4-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d28b4-153">createdDateTime</span></span>|<span data-ttu-id="d28b4-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d28b4-154">DateTimeOffset</span></span>|<span data-ttu-id="d28b4-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d28b4-155">The date and time the app was created.</span></span> <span data-ttu-id="d28b4-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d28b4-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d28b4-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d28b4-157">lastModifiedDateTime</span></span>|<span data-ttu-id="d28b4-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d28b4-158">DateTimeOffset</span></span>|<span data-ttu-id="d28b4-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="d28b4-159">The date and time the app was last modified.</span></span> <span data-ttu-id="d28b4-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d28b4-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d28b4-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d28b4-161">isFeatured</span></span>|<span data-ttu-id="d28b4-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="d28b4-162">Boolean</span></span>|<span data-ttu-id="d28b4-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d28b4-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d28b4-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d28b4-164">privacyInformationUrl</span></span>|<span data-ttu-id="d28b4-165">String</span><span class="sxs-lookup"><span data-stu-id="d28b4-165">String</span></span>|<span data-ttu-id="d28b4-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="d28b4-166">The privacy statement Url.</span></span> <span data-ttu-id="d28b4-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d28b4-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d28b4-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d28b4-168">informationUrl</span></span>|<span data-ttu-id="d28b4-169">String</span><span class="sxs-lookup"><span data-stu-id="d28b4-169">String</span></span>|<span data-ttu-id="d28b4-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="d28b4-170">The more information Url.</span></span> <span data-ttu-id="d28b4-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d28b4-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d28b4-172">owner</span><span class="sxs-lookup"><span data-stu-id="d28b4-172">owner</span></span>|<span data-ttu-id="d28b4-173">String</span><span class="sxs-lookup"><span data-stu-id="d28b4-173">String</span></span>|<span data-ttu-id="d28b4-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="d28b4-174">The owner of the app.</span></span> <span data-ttu-id="d28b4-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d28b4-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d28b4-176">developer</span><span class="sxs-lookup"><span data-stu-id="d28b4-176">developer</span></span>|<span data-ttu-id="d28b4-177">String</span><span class="sxs-lookup"><span data-stu-id="d28b4-177">String</span></span>|<span data-ttu-id="d28b4-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d28b4-178">The developer of the app.</span></span> <span data-ttu-id="d28b4-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d28b4-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d28b4-180">Observações</span><span class="sxs-lookup"><span data-stu-id="d28b4-180">notes</span></span>|<span data-ttu-id="d28b4-181">String</span><span class="sxs-lookup"><span data-stu-id="d28b4-181">String</span></span>|<span data-ttu-id="d28b4-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d28b4-182">Notes for the app.</span></span> <span data-ttu-id="d28b4-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d28b4-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d28b4-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="d28b4-184">uploadState</span></span>|<span data-ttu-id="d28b4-185">Int32</span><span class="sxs-lookup"><span data-stu-id="d28b4-185">Int32</span></span>|<span data-ttu-id="d28b4-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="d28b4-186">The upload state.</span></span> <span data-ttu-id="d28b4-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d28b4-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d28b4-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="d28b4-188">publishingState</span></span>|[<span data-ttu-id="d28b4-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="d28b4-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d28b4-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d28b4-190">The publishing state for the app.</span></span> <span data-ttu-id="d28b4-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="d28b4-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d28b4-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d28b4-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="d28b4-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="d28b4-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d28b4-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="d28b4-194">committedContentVersion</span></span>|<span data-ttu-id="d28b4-195">String</span><span class="sxs-lookup"><span data-stu-id="d28b4-195">String</span></span>|<span data-ttu-id="d28b4-196">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="d28b4-196">The internal committed content version.</span></span> <span data-ttu-id="d28b4-197">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d28b4-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d28b4-198">fileName</span><span class="sxs-lookup"><span data-stu-id="d28b4-198">fileName</span></span>|<span data-ttu-id="d28b4-199">String</span><span class="sxs-lookup"><span data-stu-id="d28b4-199">String</span></span>|<span data-ttu-id="d28b4-200">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="d28b4-200">The name of the main Lob application file.</span></span> <span data-ttu-id="d28b4-201">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d28b4-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d28b4-202">size</span><span class="sxs-lookup"><span data-stu-id="d28b4-202">size</span></span>|<span data-ttu-id="d28b4-203">Int64</span><span class="sxs-lookup"><span data-stu-id="d28b4-203">Int64</span></span>|<span data-ttu-id="d28b4-204">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="d28b4-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="d28b4-205">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d28b4-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d28b4-206">bundleId</span><span class="sxs-lookup"><span data-stu-id="d28b4-206">bundleId</span></span>|<span data-ttu-id="d28b4-207">String</span><span class="sxs-lookup"><span data-stu-id="d28b4-207">String</span></span>|<span data-ttu-id="d28b4-208">A id do pacote.</span><span class="sxs-lookup"><span data-stu-id="d28b4-208">The bundle id.</span></span>|
|<span data-ttu-id="d28b4-209">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d28b4-209">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="d28b4-210">macOSMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d28b4-210">macOSMinimumOperatingSystem</span></span>](../resources/intune-apps-macosminimumoperatingsystem.md)|<span data-ttu-id="d28b4-211">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="d28b4-211">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="d28b4-212">buildNumber</span><span class="sxs-lookup"><span data-stu-id="d28b4-212">buildNumber</span></span>|<span data-ttu-id="d28b4-213">String</span><span class="sxs-lookup"><span data-stu-id="d28b4-213">String</span></span>|<span data-ttu-id="d28b4-214">O número de compilação da linha de MacOS do aplicativo de negócios (LoB).</span><span class="sxs-lookup"><span data-stu-id="d28b4-214">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="d28b4-215">versionNumber</span><span class="sxs-lookup"><span data-stu-id="d28b4-215">versionNumber</span></span>|<span data-ttu-id="d28b4-216">String</span><span class="sxs-lookup"><span data-stu-id="d28b4-216">String</span></span>|<span data-ttu-id="d28b4-217">O número de versão da linha de MacOS do aplicativo de negócios (LoB).</span><span class="sxs-lookup"><span data-stu-id="d28b4-217">The version number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="d28b4-218">childApps</span><span class="sxs-lookup"><span data-stu-id="d28b4-218">childApps</span></span>|<span data-ttu-id="d28b4-219">coleção [macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md)</span><span class="sxs-lookup"><span data-stu-id="d28b4-219">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md) collection</span></span>|<span data-ttu-id="d28b4-220">A lista neste pacote do pacote de aplicativo</span><span class="sxs-lookup"><span data-stu-id="d28b4-220">The app list in this bundle package</span></span>|
|<span data-ttu-id="d28b4-221">identityVersion</span><span class="sxs-lookup"><span data-stu-id="d28b4-221">identityVersion</span></span>|<span data-ttu-id="d28b4-222">String</span><span class="sxs-lookup"><span data-stu-id="d28b4-222">String</span></span>|<span data-ttu-id="d28b4-223">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="d28b4-223">The identity version.</span></span>|
|<span data-ttu-id="d28b4-224">md5HashChunkSize</span><span class="sxs-lookup"><span data-stu-id="d28b4-224">md5HashChunkSize</span></span>|<span data-ttu-id="d28b4-225">Int32</span><span class="sxs-lookup"><span data-stu-id="d28b4-225">Int32</span></span>|<span data-ttu-id="d28b4-226">O tamanho do bloco de hash MD5</span><span class="sxs-lookup"><span data-stu-id="d28b4-226">The chunk size for MD5 hash</span></span>|
|<span data-ttu-id="d28b4-227">md5Hash</span><span class="sxs-lookup"><span data-stu-id="d28b4-227">md5Hash</span></span>|<span data-ttu-id="d28b4-228">String collection</span><span class="sxs-lookup"><span data-stu-id="d28b4-228">String collection</span></span>|<span data-ttu-id="d28b4-229">Os códigos de hash MD5</span><span class="sxs-lookup"><span data-stu-id="d28b4-229">The MD5 hash codes</span></span>|
|<span data-ttu-id="d28b4-230">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="d28b4-230">ignoreVersionDetection</span></span>|<span data-ttu-id="d28b4-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="d28b4-231">Boolean</span></span>|<span data-ttu-id="d28b4-232">Um booliano para controlar se a versão do aplicativo será usada para detectar o aplicativo depois que ele for instalado em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d28b4-232">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="d28b4-233">Defina essa opção para verdadeiro para macOS aplicativos de linha de negócios (LoB) que usam um recurso de atualização self.</span><span class="sxs-lookup"><span data-stu-id="d28b4-233">Set this to true for macOS Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="d28b4-234">Resposta</span><span class="sxs-lookup"><span data-stu-id="d28b4-234">Response</span></span>
<span data-ttu-id="d28b4-235">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [macOSLobApp](../resources/intune-apps-macoslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d28b4-235">If successful, this method returns a `200 OK` response code and an updated [macOSLobApp](../resources/intune-apps-macoslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d28b4-236">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d28b4-236">Example</span></span>
### <a name="request"></a><span data-ttu-id="d28b4-237">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d28b4-237">Request</span></span>
<span data-ttu-id="d28b4-238">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d28b4-238">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1476

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
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true
  },
  "buildNumber": "Build Number value",
  "versionNumber": "Version Number value",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "Bundle Id value",
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value"
    }
  ],
  "identityVersion": "Identity Version value",
  "md5HashChunkSize": 0,
  "md5Hash": [
    "Md5Hash value"
  ],
  "ignoreVersionDetection": true
}
```

### <a name="response"></a><span data-ttu-id="d28b4-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="d28b4-239">Response</span></span>
<span data-ttu-id="d28b4-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d28b4-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1634

{
  "@odata.type": "#microsoft.graph.macOSLobApp",
  "id": "7be9250a-250a-7be9-0a25-e97b0a25e97b",
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
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true
  },
  "buildNumber": "Build Number value",
  "versionNumber": "Version Number value",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "Bundle Id value",
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value"
    }
  ],
  "identityVersion": "Identity Version value",
  "md5HashChunkSize": 0,
  "md5Hash": [
    "Md5Hash value"
  ],
  "ignoreVersionDetection": true
}
```





