---
title: Criar androidLobApp
description: Cria um novo objeto androidLobApp.
author: tfitzmac
ms.openlocfilehash: 67e75c3eb8e482530a00ea7efe37a2a4ca4cb2b2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327983"
---
# <a name="create-androidlobapp"></a><span data-ttu-id="8747c-103">Criar androidLobApp</span><span class="sxs-lookup"><span data-stu-id="8747c-103">Create androidLobApp</span></span>

> <span data-ttu-id="8747c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8747c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8747c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8747c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8747c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8747c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8747c-107">Cria um novo objeto [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="8747c-107">Create a new [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8747c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8747c-108">Prerequisites</span></span>
<span data-ttu-id="8747c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8747c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8747c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8747c-111">Permission type</span></span>|<span data-ttu-id="8747c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8747c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8747c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8747c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8747c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8747c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8747c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8747c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8747c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8747c-116">Not supported.</span></span>|
|<span data-ttu-id="8747c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8747c-117">Application</span></span>|<span data-ttu-id="8747c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8747c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8747c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8747c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="8747c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8747c-120">Request headers</span></span>
|<span data-ttu-id="8747c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8747c-121">Header</span></span>|<span data-ttu-id="8747c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8747c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8747c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8747c-123">Authorization</span></span>|<span data-ttu-id="8747c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8747c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8747c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8747c-125">Accept</span></span>|<span data-ttu-id="8747c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8747c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8747c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8747c-127">Request body</span></span>
<span data-ttu-id="8747c-128">No corpo da solicitação, forneça uma representação JSON do objeto androidLobApp.</span><span class="sxs-lookup"><span data-stu-id="8747c-128">In the request body, supply a JSON representation for the androidLobApp object.</span></span>

<span data-ttu-id="8747c-129">A tabela a seguir mostra as propriedades obrigatórias ao criar androidLobApp.</span><span class="sxs-lookup"><span data-stu-id="8747c-129">The following table shows the properties that are required when you create the androidLobApp.</span></span>

|<span data-ttu-id="8747c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8747c-130">Property</span></span>|<span data-ttu-id="8747c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8747c-131">Type</span></span>|<span data-ttu-id="8747c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8747c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8747c-133">id</span><span class="sxs-lookup"><span data-stu-id="8747c-133">id</span></span>|<span data-ttu-id="8747c-134">String</span><span class="sxs-lookup"><span data-stu-id="8747c-134">String</span></span>|<span data-ttu-id="8747c-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8747c-135">Key of the entity.</span></span> <span data-ttu-id="8747c-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8747c-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8747c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="8747c-137">displayName</span></span>|<span data-ttu-id="8747c-138">String</span><span class="sxs-lookup"><span data-stu-id="8747c-138">String</span></span>|<span data-ttu-id="8747c-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="8747c-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8747c-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8747c-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8747c-141">description</span><span class="sxs-lookup"><span data-stu-id="8747c-141">description</span></span>|<span data-ttu-id="8747c-142">String</span><span class="sxs-lookup"><span data-stu-id="8747c-142">String</span></span>|<span data-ttu-id="8747c-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8747c-143">The description of the app.</span></span> <span data-ttu-id="8747c-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8747c-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8747c-145">publisher</span><span class="sxs-lookup"><span data-stu-id="8747c-145">publisher</span></span>|<span data-ttu-id="8747c-146">String</span><span class="sxs-lookup"><span data-stu-id="8747c-146">String</span></span>|<span data-ttu-id="8747c-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8747c-147">The publisher of the app.</span></span> <span data-ttu-id="8747c-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8747c-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8747c-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8747c-149">largeIcon</span></span>|[<span data-ttu-id="8747c-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8747c-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8747c-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="8747c-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8747c-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8747c-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8747c-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8747c-153">createdDateTime</span></span>|<span data-ttu-id="8747c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8747c-154">DateTimeOffset</span></span>|<span data-ttu-id="8747c-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8747c-155">The date and time the app was created.</span></span> <span data-ttu-id="8747c-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8747c-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8747c-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8747c-157">lastModifiedDateTime</span></span>|<span data-ttu-id="8747c-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8747c-158">DateTimeOffset</span></span>|<span data-ttu-id="8747c-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8747c-159">The date and time the app was last modified.</span></span> <span data-ttu-id="8747c-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8747c-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8747c-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8747c-161">isFeatured</span></span>|<span data-ttu-id="8747c-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="8747c-162">Boolean</span></span>|<span data-ttu-id="8747c-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8747c-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8747c-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8747c-164">privacyInformationUrl</span></span>|<span data-ttu-id="8747c-165">String</span><span class="sxs-lookup"><span data-stu-id="8747c-165">String</span></span>|<span data-ttu-id="8747c-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="8747c-166">The privacy statement Url.</span></span> <span data-ttu-id="8747c-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8747c-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8747c-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8747c-168">informationUrl</span></span>|<span data-ttu-id="8747c-169">String</span><span class="sxs-lookup"><span data-stu-id="8747c-169">String</span></span>|<span data-ttu-id="8747c-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="8747c-170">The more information Url.</span></span> <span data-ttu-id="8747c-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8747c-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8747c-172">owner</span><span class="sxs-lookup"><span data-stu-id="8747c-172">owner</span></span>|<span data-ttu-id="8747c-173">String</span><span class="sxs-lookup"><span data-stu-id="8747c-173">String</span></span>|<span data-ttu-id="8747c-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="8747c-174">The owner of the app.</span></span> <span data-ttu-id="8747c-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8747c-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8747c-176">developer</span><span class="sxs-lookup"><span data-stu-id="8747c-176">developer</span></span>|<span data-ttu-id="8747c-177">String</span><span class="sxs-lookup"><span data-stu-id="8747c-177">String</span></span>|<span data-ttu-id="8747c-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8747c-178">The developer of the app.</span></span> <span data-ttu-id="8747c-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8747c-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8747c-180">Observações</span><span class="sxs-lookup"><span data-stu-id="8747c-180">notes</span></span>|<span data-ttu-id="8747c-181">String</span><span class="sxs-lookup"><span data-stu-id="8747c-181">String</span></span>|<span data-ttu-id="8747c-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8747c-182">Notes for the app.</span></span> <span data-ttu-id="8747c-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8747c-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8747c-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="8747c-184">uploadState</span></span>|<span data-ttu-id="8747c-185">Int32</span><span class="sxs-lookup"><span data-stu-id="8747c-185">Int32</span></span>|<span data-ttu-id="8747c-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="8747c-186">The upload state.</span></span> <span data-ttu-id="8747c-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8747c-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8747c-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="8747c-188">publishingState</span></span>|[<span data-ttu-id="8747c-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="8747c-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8747c-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8747c-190">The publishing state for the app.</span></span> <span data-ttu-id="8747c-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="8747c-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8747c-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8747c-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="8747c-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="8747c-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8747c-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="8747c-194">committedContentVersion</span></span>|<span data-ttu-id="8747c-195">String</span><span class="sxs-lookup"><span data-stu-id="8747c-195">String</span></span>|<span data-ttu-id="8747c-196">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="8747c-196">The internal committed content version.</span></span> <span data-ttu-id="8747c-197">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="8747c-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="8747c-198">fileName</span><span class="sxs-lookup"><span data-stu-id="8747c-198">fileName</span></span>|<span data-ttu-id="8747c-199">String</span><span class="sxs-lookup"><span data-stu-id="8747c-199">String</span></span>|<span data-ttu-id="8747c-200">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="8747c-200">The name of the main Lob application file.</span></span> <span data-ttu-id="8747c-201">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="8747c-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="8747c-202">size</span><span class="sxs-lookup"><span data-stu-id="8747c-202">size</span></span>|<span data-ttu-id="8747c-203">Int64</span><span class="sxs-lookup"><span data-stu-id="8747c-203">Int64</span></span>|<span data-ttu-id="8747c-204">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="8747c-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="8747c-205">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="8747c-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="8747c-206">packageId</span><span class="sxs-lookup"><span data-stu-id="8747c-206">packageId</span></span>|<span data-ttu-id="8747c-207">String</span><span class="sxs-lookup"><span data-stu-id="8747c-207">String</span></span>|<span data-ttu-id="8747c-208">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="8747c-208">The package identifier.</span></span>|
|<span data-ttu-id="8747c-209">identityName</span><span class="sxs-lookup"><span data-stu-id="8747c-209">identityName</span></span>|<span data-ttu-id="8747c-210">String</span><span class="sxs-lookup"><span data-stu-id="8747c-210">String</span></span>|<span data-ttu-id="8747c-211">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="8747c-211">The Identity Name.</span></span>|
|<span data-ttu-id="8747c-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8747c-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="8747c-213">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8747c-213">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="8747c-214">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="8747c-214">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="8747c-215">versionName</span><span class="sxs-lookup"><span data-stu-id="8747c-215">versionName</span></span>|<span data-ttu-id="8747c-216">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8747c-216">String</span></span>|<span data-ttu-id="8747c-217">O nome da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="8747c-217">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="8747c-218">versionCode</span><span class="sxs-lookup"><span data-stu-id="8747c-218">versionCode</span></span>|<span data-ttu-id="8747c-219">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8747c-219">String</span></span>|<span data-ttu-id="8747c-220">O código da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="8747c-220">The version code of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="8747c-221">identityVersion</span><span class="sxs-lookup"><span data-stu-id="8747c-221">identityVersion</span></span>|<span data-ttu-id="8747c-222">String</span><span class="sxs-lookup"><span data-stu-id="8747c-222">String</span></span>|<span data-ttu-id="8747c-223">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="8747c-223">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="8747c-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="8747c-224">Response</span></span>
<span data-ttu-id="8747c-225">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [androidLobApp](../resources/intune-apps-androidlobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8747c-225">If successful, this method returns a `201 Created` response code and a [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8747c-226">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8747c-226">Example</span></span>
### <a name="request"></a><span data-ttu-id="8747c-227">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8747c-227">Request</span></span>
<span data-ttu-id="8747c-228">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8747c-228">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1365

{
  "@odata.type": "#microsoft.graph.androidLobApp",
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

### <a name="response"></a><span data-ttu-id="8747c-229">Resposta</span><span class="sxs-lookup"><span data-stu-id="8747c-229">Response</span></span>
<span data-ttu-id="8747c-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8747c-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





