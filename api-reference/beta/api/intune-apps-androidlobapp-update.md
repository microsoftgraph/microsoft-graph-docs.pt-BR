---
title: Atualizar androidLobApp
description: Atualiza as propriedades de um objeto androidLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 81479b93cd24ec0597c55ccf53692af16b63de94
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925970"
---
# <a name="update-androidlobapp"></a><span data-ttu-id="8832a-103">Atualizar androidLobApp</span><span class="sxs-lookup"><span data-stu-id="8832a-103">Update androidLobApp</span></span>

> <span data-ttu-id="8832a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8832a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8832a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8832a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8832a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8832a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8832a-107">Atualiza as propriedades de um objeto [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="8832a-107">Update the properties of a [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8832a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8832a-108">Prerequisites</span></span>
<span data-ttu-id="8832a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8832a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8832a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8832a-111">Permission type</span></span>|<span data-ttu-id="8832a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8832a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8832a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8832a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8832a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8832a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8832a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8832a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8832a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8832a-116">Not supported.</span></span>|
|<span data-ttu-id="8832a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8832a-117">Application</span></span>|<span data-ttu-id="8832a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8832a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8832a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8832a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="8832a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8832a-120">Request headers</span></span>
|<span data-ttu-id="8832a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8832a-121">Header</span></span>|<span data-ttu-id="8832a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8832a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8832a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8832a-123">Authorization</span></span>|<span data-ttu-id="8832a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8832a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8832a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8832a-125">Accept</span></span>|<span data-ttu-id="8832a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8832a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8832a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8832a-127">Request body</span></span>
<span data-ttu-id="8832a-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="8832a-128">In the request body, supply a JSON representation for the [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

<span data-ttu-id="8832a-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="8832a-129">The following table shows the properties that are required when you create the [androidLobApp](../resources/intune-apps-androidlobapp.md).</span></span>

|<span data-ttu-id="8832a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8832a-130">Property</span></span>|<span data-ttu-id="8832a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8832a-131">Type</span></span>|<span data-ttu-id="8832a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8832a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8832a-133">id</span><span class="sxs-lookup"><span data-stu-id="8832a-133">id</span></span>|<span data-ttu-id="8832a-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8832a-134">String</span></span>|<span data-ttu-id="8832a-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8832a-135">Key of the entity.</span></span> <span data-ttu-id="8832a-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8832a-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8832a-137">displayName</span><span class="sxs-lookup"><span data-stu-id="8832a-137">displayName</span></span>|<span data-ttu-id="8832a-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8832a-138">String</span></span>|<span data-ttu-id="8832a-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="8832a-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8832a-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8832a-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8832a-141">description</span><span class="sxs-lookup"><span data-stu-id="8832a-141">description</span></span>|<span data-ttu-id="8832a-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8832a-142">String</span></span>|<span data-ttu-id="8832a-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8832a-143">The description of the app.</span></span> <span data-ttu-id="8832a-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8832a-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8832a-145">publisher</span><span class="sxs-lookup"><span data-stu-id="8832a-145">publisher</span></span>|<span data-ttu-id="8832a-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8832a-146">String</span></span>|<span data-ttu-id="8832a-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8832a-147">The publisher of the app.</span></span> <span data-ttu-id="8832a-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8832a-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8832a-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8832a-149">largeIcon</span></span>|[<span data-ttu-id="8832a-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8832a-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8832a-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="8832a-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8832a-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8832a-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8832a-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8832a-153">createdDateTime</span></span>|<span data-ttu-id="8832a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8832a-154">DateTimeOffset</span></span>|<span data-ttu-id="8832a-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8832a-155">The date and time the app was created.</span></span> <span data-ttu-id="8832a-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8832a-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8832a-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8832a-157">lastModifiedDateTime</span></span>|<span data-ttu-id="8832a-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8832a-158">DateTimeOffset</span></span>|<span data-ttu-id="8832a-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8832a-159">The date and time the app was last modified.</span></span> <span data-ttu-id="8832a-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8832a-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8832a-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8832a-161">isFeatured</span></span>|<span data-ttu-id="8832a-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="8832a-162">Boolean</span></span>|<span data-ttu-id="8832a-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8832a-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8832a-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8832a-164">privacyInformationUrl</span></span>|<span data-ttu-id="8832a-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8832a-165">String</span></span>|<span data-ttu-id="8832a-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="8832a-166">The privacy statement Url.</span></span> <span data-ttu-id="8832a-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8832a-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8832a-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8832a-168">informationUrl</span></span>|<span data-ttu-id="8832a-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8832a-169">String</span></span>|<span data-ttu-id="8832a-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="8832a-170">The more information Url.</span></span> <span data-ttu-id="8832a-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8832a-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8832a-172">owner</span><span class="sxs-lookup"><span data-stu-id="8832a-172">owner</span></span>|<span data-ttu-id="8832a-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8832a-173">String</span></span>|<span data-ttu-id="8832a-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="8832a-174">The owner of the app.</span></span> <span data-ttu-id="8832a-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8832a-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8832a-176">developer</span><span class="sxs-lookup"><span data-stu-id="8832a-176">developer</span></span>|<span data-ttu-id="8832a-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8832a-177">String</span></span>|<span data-ttu-id="8832a-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8832a-178">The developer of the app.</span></span> <span data-ttu-id="8832a-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8832a-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8832a-180">Observações</span><span class="sxs-lookup"><span data-stu-id="8832a-180">notes</span></span>|<span data-ttu-id="8832a-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8832a-181">String</span></span>|<span data-ttu-id="8832a-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8832a-182">Notes for the app.</span></span> <span data-ttu-id="8832a-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8832a-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8832a-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="8832a-184">uploadState</span></span>|<span data-ttu-id="8832a-185">Int32</span><span class="sxs-lookup"><span data-stu-id="8832a-185">Int32</span></span>|<span data-ttu-id="8832a-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="8832a-186">The upload state.</span></span> <span data-ttu-id="8832a-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8832a-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8832a-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="8832a-188">publishingState</span></span>|[<span data-ttu-id="8832a-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="8832a-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8832a-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8832a-190">The publishing state for the app.</span></span> <span data-ttu-id="8832a-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="8832a-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8832a-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8832a-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="8832a-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="8832a-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8832a-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="8832a-194">committedContentVersion</span></span>|<span data-ttu-id="8832a-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8832a-195">String</span></span>|<span data-ttu-id="8832a-196">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="8832a-196">The internal committed content version.</span></span> <span data-ttu-id="8832a-197">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="8832a-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="8832a-198">fileName</span><span class="sxs-lookup"><span data-stu-id="8832a-198">fileName</span></span>|<span data-ttu-id="8832a-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8832a-199">String</span></span>|<span data-ttu-id="8832a-200">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="8832a-200">The name of the main Lob application file.</span></span> <span data-ttu-id="8832a-201">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="8832a-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="8832a-202">size</span><span class="sxs-lookup"><span data-stu-id="8832a-202">size</span></span>|<span data-ttu-id="8832a-203">Int64</span><span class="sxs-lookup"><span data-stu-id="8832a-203">Int64</span></span>|<span data-ttu-id="8832a-204">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="8832a-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="8832a-205">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="8832a-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="8832a-206">packageId</span><span class="sxs-lookup"><span data-stu-id="8832a-206">packageId</span></span>|<span data-ttu-id="8832a-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8832a-207">String</span></span>|<span data-ttu-id="8832a-208">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="8832a-208">The package identifier.</span></span>|
|<span data-ttu-id="8832a-209">identityName</span><span class="sxs-lookup"><span data-stu-id="8832a-209">identityName</span></span>|<span data-ttu-id="8832a-210">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8832a-210">String</span></span>|<span data-ttu-id="8832a-211">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="8832a-211">The Identity Name.</span></span>|
|<span data-ttu-id="8832a-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8832a-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="8832a-213">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8832a-213">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="8832a-214">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="8832a-214">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="8832a-215">versionName</span><span class="sxs-lookup"><span data-stu-id="8832a-215">versionName</span></span>|<span data-ttu-id="8832a-216">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8832a-216">String</span></span>|<span data-ttu-id="8832a-217">O nome da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="8832a-217">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="8832a-218">versionCode</span><span class="sxs-lookup"><span data-stu-id="8832a-218">versionCode</span></span>|<span data-ttu-id="8832a-219">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8832a-219">String</span></span>|<span data-ttu-id="8832a-220">O código da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="8832a-220">The version code of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="8832a-221">identityVersion</span><span class="sxs-lookup"><span data-stu-id="8832a-221">identityVersion</span></span>|<span data-ttu-id="8832a-222">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8832a-222">String</span></span>|<span data-ttu-id="8832a-223">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="8832a-223">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="8832a-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="8832a-224">Response</span></span>
<span data-ttu-id="8832a-225">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [androidLobApp](../resources/intune-apps-androidlobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8832a-225">If successful, this method returns a `200 OK` response code and an updated [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8832a-226">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8832a-226">Example</span></span>
### <a name="request"></a><span data-ttu-id="8832a-227">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8832a-227">Request</span></span>
<span data-ttu-id="8832a-228">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8832a-228">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1313

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
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="8832a-229">Resposta</span><span class="sxs-lookup"><span data-stu-id="8832a-229">Response</span></span>
<span data-ttu-id="8832a-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8832a-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1473

{
  "@odata.type": "#microsoft.graph.androidLobApp",
  "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```





