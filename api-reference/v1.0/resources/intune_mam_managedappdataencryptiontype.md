# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="901f7-101">tipo de enumeração managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="901f7-101">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="901f7-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="901f7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="901f7-103">Representa o nível ao qual os dados de aplicativo são criptografados para aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="901f7-103">Represents the level to which app data is encrypted for managed apps</span></span>
## <a name="members"></a><span data-ttu-id="901f7-104">Membros</span><span class="sxs-lookup"><span data-stu-id="901f7-104">Members</span></span>
|<span data-ttu-id="901f7-105">Membro</span><span class="sxs-lookup"><span data-stu-id="901f7-105">Member</span></span>|<span data-ttu-id="901f7-106">Valor</span><span class="sxs-lookup"><span data-stu-id="901f7-106">Value</span></span>|<span data-ttu-id="901f7-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="901f7-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="901f7-108">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="901f7-108">useDeviceSettings</span></span>|<span data-ttu-id="901f7-109">0</span><span class="sxs-lookup"><span data-stu-id="901f7-109">0%</span></span>|<span data-ttu-id="901f7-110">Os dados do aplicativo são criptografados com base nas configurações padrão do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="901f7-110">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="901f7-111">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="901f7-111">afterDeviceRestart</span></span>|<span data-ttu-id="901f7-112">1</span><span class="sxs-lookup"><span data-stu-id="901f7-112">-1</span></span>|<span data-ttu-id="901f7-113">Os dados do aplicativo são criptografados quando o dispositivo for reiniciado.</span><span class="sxs-lookup"><span data-stu-id="901f7-113">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="901f7-114">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="901f7-114">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="901f7-115">2</span><span class="sxs-lookup"><span data-stu-id="901f7-115">-2</span></span>|<span data-ttu-id="901f7-116">Os dados de aplicativo associados a essa política são criptografados quando o dispositivo for bloqueado, exceto os dados em arquivos que estão abertos</span><span class="sxs-lookup"><span data-stu-id="901f7-116">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="901f7-117">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="901f7-117">whenDeviceLocked</span></span>|<span data-ttu-id="901f7-118">3</span><span class="sxs-lookup"><span data-stu-id="901f7-118">-3</span></span>|<span data-ttu-id="901f7-119">Os dados do aplicativo associados a essa política são criptografados quando o dispositivo for bloqueado</span><span class="sxs-lookup"><span data-stu-id="901f7-119">App data associated with this policy is encrypted when the device is locked</span></span>|








