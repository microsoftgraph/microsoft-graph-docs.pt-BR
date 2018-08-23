# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="044a2-101">tipo de enumeração mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="044a2-101">mobileAppPublishingState enum type</span></span>

> <span data-ttu-id="044a2-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="044a2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="044a2-103">Indica o estado de publicação de um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="044a2-103">Indicates the publishing state of an app.</span></span>
## <a name="members"></a><span data-ttu-id="044a2-104">Membros</span><span class="sxs-lookup"><span data-stu-id="044a2-104">Members</span></span>
|<span data-ttu-id="044a2-105">Membro</span><span class="sxs-lookup"><span data-stu-id="044a2-105">Member</span></span>|<span data-ttu-id="044a2-106">Valor</span><span class="sxs-lookup"><span data-stu-id="044a2-106">Value</span></span>|<span data-ttu-id="044a2-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="044a2-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="044a2-108">notPublished</span><span class="sxs-lookup"><span data-stu-id="044a2-108">notPublished</span></span>|<span data-ttu-id="044a2-109">0</span><span class="sxs-lookup"><span data-stu-id="044a2-109">0%</span></span>|<span data-ttu-id="044a2-110">O aplicativo ainda não foi publicado.</span><span class="sxs-lookup"><span data-stu-id="044a2-110">The app is not yet published.</span></span>|
|<span data-ttu-id="044a2-111">processamento</span><span class="sxs-lookup"><span data-stu-id="044a2-111">Processing</span></span>|<span data-ttu-id="044a2-112">1</span><span class="sxs-lookup"><span data-stu-id="044a2-112">$1</span></span>|<span data-ttu-id="044a2-113">O aplicativo está aguardando processamento no lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="044a2-113">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="044a2-114">publicado</span><span class="sxs-lookup"><span data-stu-id="044a2-114">published</span></span>|<span data-ttu-id="044a2-115">2</span><span class="sxs-lookup"><span data-stu-id="044a2-115">-2</span></span>|<span data-ttu-id="044a2-116">O aplicativo foi publicado.</span><span class="sxs-lookup"><span data-stu-id="044a2-116">The app is removed.</span></span>|



