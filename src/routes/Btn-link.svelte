<script>
    export let text = 'text';
</script>

<a href="http://example.com">
    <div class="link-btn accented-body-s">
        {text}
    </div>
</a>

<style>
    .link-btn {
        display: flex;
        padding: 6px 16px;
        align-items: flex-start;
        border-radius: 40px;
        background: rgba(100, 43, 255, 0.10);
        font-size: 15px;
        line-height: 28px;
        font-weight: 500;
        border:2px solid transparent;
        white-space: nowrap;
    }
    .link-btn:hover {
        border:2px solid #622bff;
        transition: 0.3s ease-in-out;
    }
</style>